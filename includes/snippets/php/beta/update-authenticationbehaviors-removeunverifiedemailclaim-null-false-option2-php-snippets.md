---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

<?php

// THIS SNIPPET IS A PREVIEW VERSION OF THE SDK. NON-PRODUCTION USE ONLY
$graphServiceClient = new GraphServiceClient($tokenRequestContext, $scopes);

$requestBody = new Application();
$authenticationBehaviors = new AuthenticationBehaviors();
$AuthenticationBehaviors->setRemoveUnverifiedEmailClaim(null);
$requestBody->setAuthenticationBehaviors($authenticationBehaviors);

$result = $graphServiceClient->applications()->byApplicationId('application-id')->patch($requestBody)->wait();

```