---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0346b8fd811fbf6587b73ef19e993771dfe990f4
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48953530"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

B2cIdentityUserFlow b2cIdentityUserFlow = new B2cIdentityUserFlow();
b2cIdentityUserFlow.id = "Customer";
b2cIdentityUserFlow.userFlowType = UserFlowType.SIGN_UP_OR_SIGN_IN;
b2cIdentityUserFlow.userFlowTypeVersion = 3;
LinkedList<IdentityProvider> identityProvidersList = new LinkedList<IdentityProvider>();
IdentityProvider identityProviders = new IdentityProvider();
identityProviders.id = "Facebook-OAuth";
identityProviders.type = "Facebook";
identityProviders.Name = "Facebook";
identityProvidersList.add(identityProviders);
IdentityProviderCollectionResponse identityProviderCollectionResponse = new IdentityProviderCollectionResponse();
identityProviderCollectionResponse.value = identityProvidersList;
IdentityProviderCollectionPage identityProviderCollectionPage = new IdentityProviderCollectionPage(identityProviderCollectionResponse, null);
b2cIdentityUserFlow.identityProviders = identityProviderCollectionPage;

graphClient.identity().b2cUserFlows()
    .buildRequest()
    .post(b2cIdentityUserFlow);

```