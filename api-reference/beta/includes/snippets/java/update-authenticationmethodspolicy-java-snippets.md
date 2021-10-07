---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b615f574c4ecfe214c1671d9acd2ec5a628c35ec018133f7bf3aab87bc559fed
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105664"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AuthenticationMethodsPolicy authenticationMethodsPolicy = new AuthenticationMethodsPolicy();
RegistrationEnforcement registrationEnforcement = new RegistrationEnforcement();
AuthenticationMethodsRegistrationCampaign authenticationMethodsRegistrationCampaign = new AuthenticationMethodsRegistrationCampaign();
authenticationMethodsRegistrationCampaign.snoozeDurationInDays = 1;
authenticationMethodsRegistrationCampaign.state = AdvancedConfigState.ENABLED;
LinkedList<ExcludeTarget> excludeTargetsList = new LinkedList<ExcludeTarget>();
authenticationMethodsRegistrationCampaign.excludeTargets = excludeTargetsList;
LinkedList<AuthenticationMethodsRegistrationCampaignIncludeTarget> includeTargetsList = new LinkedList<AuthenticationMethodsRegistrationCampaignIncludeTarget>();
AuthenticationMethodsRegistrationCampaignIncludeTarget includeTargets = new AuthenticationMethodsRegistrationCampaignIncludeTarget();
includeTargets.id = "3ee3a9de-0a86-4e12-a287-9769accf1ba2";
includeTargets.targetType = AuthenticationMethodTargetType.GROUP;
includeTargets.targetedAuthenticationMethod = "microsoftAuthenticator";
includeTargetsList.add(includeTargets);
authenticationMethodsRegistrationCampaign.includeTargets = includeTargetsList;
registrationEnforcement.authenticationMethodsRegistrationCampaign = authenticationMethodsRegistrationCampaign;
authenticationMethodsPolicy.registrationEnforcement = registrationEnforcement;

graphClient.policies().authenticationMethodsPolicy()
    .buildRequest()
    .patch(authenticationMethodsPolicy);

```