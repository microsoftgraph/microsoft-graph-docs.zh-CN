---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6e13c4ca70e608cc63ce6d56cf3fbeee15f7a254
ms.sourcegitcommit: 5bb981b4853663354a566d4a4a5cbf288939e441
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2021
ms.locfileid: "53580829"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AuthenticationMethodsPolicy authenticationMethodsPolicy = new AuthenticationMethodsPolicy();
authenticationMethodsPolicy.additionalDataManager().put("@odata.context", new JsonPrimitive("https://graph.microsoft.com/v1.0/$metadata#authenticationMethodsPolicy"));
LinkedList<AuthenticationMethodConfiguration> authenticationMethodConfigurationsList = new LinkedList<AuthenticationMethodConfiguration>();
Fido2AuthenticationMethodConfiguration authenticationMethodConfigurations = new Fido2AuthenticationMethodConfiguration();
authenticationMethodConfigurations.id = "Fido2";
authenticationMethodConfigurations.state = AuthenticationMethodState.DISABLED;
authenticationMethodConfigurations.isSelfServiceRegistrationAllowed = false;
authenticationMethodConfigurations.isAttestationEnforced = false;
Fido2KeyRestrictions keyRestrictions = new Fido2KeyRestrictions();
keyRestrictions.isEnforced = false;
keyRestrictions.enforcementType = Fido2RestrictionEnforcementType.BLOCK;
LinkedList<String> aaGuidsList = new LinkedList<String>();
keyRestrictions.aaGuids = aaGuidsList;
authenticationMethodConfigurations.keyRestrictions = keyRestrictions;
authenticationMethodConfigurationsList.add(authenticationMethodConfigurations);
AuthenticationMethodConfigurationCollectionResponse authenticationMethodConfigurationCollectionResponse = new AuthenticationMethodConfigurationCollectionResponse();
authenticationMethodConfigurationCollectionResponse.value = authenticationMethodConfigurationsList;
AuthenticationMethodConfigurationCollectionPage authenticationMethodConfigurationCollectionPage = new AuthenticationMethodConfigurationCollectionPage(authenticationMethodConfigurationCollectionResponse, null);
authenticationMethodsPolicy.authenticationMethodConfigurations = authenticationMethodConfigurationCollectionPage;

graphClient.policies().authenticationMethodsPolicy()
    .buildRequest()
    .patch(authenticationMethodsPolicy);

```