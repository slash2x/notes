## This one error
	Accounts.loginServiceConfiguration.remove({
		service: "facebook"
	});

	Accounts.loginServiceConfiguration.insert({
		service: "facebook",
		clientId: "506442426063931",
		secret: "3c1e65fd698c11b2765b9f4a678729e7"
	});

## This one Works!
	Accounts.loginServiceConfiguration.remove({
		service: "facebook"
	});

	Accounts.loginServiceConfiguration.insert({
		service: "facebook",
		appId: "506442426063931",
		secret: "3c1e65fd698c11b2765b9f4a678729e7"
	});

## You should use appId in fb login, not clientId