---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5617ddbda4e14f9d13c1fae1a654330281add8e43de018383765c37c9d62994b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332660"
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