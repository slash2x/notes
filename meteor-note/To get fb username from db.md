# To get fb username from db
## server :
	Meteor.publish("pp_url", function () {
	  return Meteor.users.find({_id: this.userId},
	         {fields:{'services.facebook.username': 1}});
	});

## client :
	Meteor.subscribe('pp_url');
	var fbdata = Meteor.users.findOne();
	console.log(fbdata.services.facebook.username);