---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a2e574d30b9ae1a61079cb8a16e105b735a649f0da799e279f221e28a46a559c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161436"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

B2cIdentityUserFlow b2cIdentityUserFlow = new B2cIdentityUserFlow();
b2cIdentityUserFlow.id = "UserFlowWithAPIConnector";
b2cIdentityUserFlow.userFlowType = UserFlowType.SIGN_UP_OR_SIGN_IN;
b2cIdentityUserFlow.userFlowTypeVersion = 1;
UserFlowApiConnectorConfiguration apiConnectorConfiguration = new UserFlowApiConnectorConfiguration();
IdentityApiConnector postFederationSignup = new IdentityApiConnector();
postFederationSignup.additionalDataManager().put("@odata.id", new JsonPrimitive("{apiConnectorId}"));
apiConnectorConfiguration.postFederationSignup = postFederationSignup;
IdentityApiConnector postAttributeCollection = new IdentityApiConnector();
postAttributeCollection.additionalDataManager().put("@odata.id", new JsonPrimitive("{apiConnectorId}"));
apiConnectorConfiguration.postAttributeCollection = postAttributeCollection;
b2cIdentityUserFlow.apiConnectorConfiguration = apiConnectorConfiguration;

graphClient.identity().b2cUserFlows()
    .buildRequest()
    .post(b2cIdentityUserFlow);

```