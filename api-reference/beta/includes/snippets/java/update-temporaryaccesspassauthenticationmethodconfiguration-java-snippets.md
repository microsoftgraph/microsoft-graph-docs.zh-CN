---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 37b2ee56bfbd6006054d3d2c8c267a02b363cacd
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50980271"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TemporaryAccessPassAuthenticationMethodConfiguration authenticationMethodConfiguration = new TemporaryAccessPassAuthenticationMethodConfiguration();
authenticationMethodConfiguration.state = AuthenticationMethodState.ENABLED;
authenticationMethodConfiguration.defaultLifetimeInMinutes = 60;
authenticationMethodConfiguration.defaultLength = 8;
authenticationMethodConfiguration.minimumLifetimeInMinutes = 60;
authenticationMethodConfiguration.maximumLifetimeInMinutes = 1440;
authenticationMethodConfiguration.
  isUsableOnce = false;
LinkedList<AuthenticationMethodTarget> includeTargetsList = new LinkedList<AuthenticationMethodTarget>();
AuthenticationMethodTarget includeTargets = new AuthenticationMethodTarget();
includeTargets.targetType = AuthenticationMethodTargetType.GROUP;
includeTargets.id = "all_users";
includeTargets.isRegistrationRequired = false;
includeTargets.useForSignIn = true;
includeTargetsList.add(includeTargets);
AuthenticationMethodTargetCollectionResponse authenticationMethodTargetCollectionResponse = new AuthenticationMethodTargetCollectionResponse();
authenticationMethodTargetCollectionResponse.value = includeTargetsList;
AuthenticationMethodTargetCollectionPage authenticationMethodTargetCollectionPage = new AuthenticationMethodTargetCollectionPage(authenticationMethodTargetCollectionResponse, null);
authenticationMethodConfiguration.includeTargets = authenticationMethodTargetCollectionPage;

graphClient.policies().authenticationMethodsPolicy().authenticationMethodConfigurations("TemporaryAccessPass")
    .buildRequest()
    .patch(authenticationMethodConfiguration);

```