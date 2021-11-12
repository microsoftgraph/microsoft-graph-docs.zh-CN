---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 37072cb5acd0e7df6221469206c1cb15afd9bcb20a611e68eb32a592a54cd84a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221109"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

B2xIdentityUserFlow b2xIdentityUserFlow = new B2xIdentityUserFlow();
b2xIdentityUserFlow.id = "UserFlowWithAPIConnector";
b2xIdentityUserFlow.userFlowType = UserFlowType.SIGN_UP_OR_SIGN_IN;
b2xIdentityUserFlow.userFlowTypeVersion = 1;
UserFlowApiConnectorConfiguration apiConnectorConfiguration = new UserFlowApiConnectorConfiguration();
IdentityApiConnector postFederationSignup = new IdentityApiConnector();
postFederationSignup.additionalDataManager().put("@odata.id", new JsonPrimitive("{apiConnectorId}"));
apiConnectorConfiguration.postFederationSignup = postFederationSignup;
IdentityApiConnector postAttributeCollection = new IdentityApiConnector();
postAttributeCollection.additionalDataManager().put("@odata.id", new JsonPrimitive("{apiConnectorId}"));
apiConnectorConfiguration.postAttributeCollection = postAttributeCollection;
b2xIdentityUserFlow.apiConnectorConfiguration = apiConnectorConfiguration;

graphClient.identity().b2xUserFlows()
    .buildRequest()
    .post(b2xIdentityUserFlow);

```