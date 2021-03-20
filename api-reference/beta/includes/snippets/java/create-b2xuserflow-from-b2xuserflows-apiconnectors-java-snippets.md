---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: febebf2d4441f70c5aa91f6c2519499446e0d618
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50975294"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

B2xIdentityUserFlow b2xIdentityUserFlow = new B2xIdentityUserFlow();
b2xIdentityUserFlow.id = "UserFlowWithAPIConnector";
b2xIdentityUserFlow.userFlowType = UserFlowType.SIGN_UP_OR_SIGN_IN;
b2xIdentityUserFlow.userFlowTypeVersion = 1;
UserFlowApiConnectorConfiguration apiConnectorConfiguration = new UserFlowApiConnectorConfiguration();
IdentityApiConnector postFederationSignup = new IdentityApiConnector();
postFederationSignup.additionalDataManager().put("@odata.id", new JsonPrimitive("https://graph.microsoft.com/beta/identity/apiConnectors/{id}"));
apiConnectorConfiguration.postFederationSignup = postFederationSignup;
IdentityApiConnector postAttributeCollection = new IdentityApiConnector();
postAttributeCollection.additionalDataManager().put("@odata.id", new JsonPrimitive("https://graph.microsoft.com/beta/identity/apiConnectors/{id}"));
apiConnectorConfiguration.postAttributeCollection = postAttributeCollection;
b2xIdentityUserFlow.apiConnectorConfiguration = apiConnectorConfiguration;

graphClient.identity().b2xUserFlows()
    .buildRequest()
    .post(b2xIdentityUserFlow);

```