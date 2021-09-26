---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1a3c1bfc341821cd875a1f039dd6d8aa936257b1
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59763500"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("Location", "https://graph.microsoft.com/beta/identity/b2cUserFlows('B2C_1_Customer')"));

B2cIdentityUserFlow b2cIdentityUserFlow = new B2cIdentityUserFlow();
b2cIdentityUserFlow.id = "Customer";
b2cIdentityUserFlow.userFlowType = UserFlowType.SIGN_UP_OR_SIGN_IN;
b2cIdentityUserFlow.userFlowTypeVersion = 3;
LinkedList<IdentityProvider> identityProvidersList = new LinkedList<IdentityProvider>();
IdentityProvider identityProviders = new IdentityProvider();
identityProviders.id = "Facebook-OAuth";
identityProvidersList.add(identityProviders);
IdentityProviderCollectionResponse identityProviderCollectionResponse = new IdentityProviderCollectionResponse();
identityProviderCollectionResponse.value = identityProvidersList;
IdentityProviderCollectionPage identityProviderCollectionPage = new IdentityProviderCollectionPage(identityProviderCollectionResponse, null);
b2cIdentityUserFlow.identityProviders = identityProviderCollectionPage;

graphClient.identity().b2cUserFlows()
    .buildRequest( requestOptions )
    .post(b2cIdentityUserFlow);

```