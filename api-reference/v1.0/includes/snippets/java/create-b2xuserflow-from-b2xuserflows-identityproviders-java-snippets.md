---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9582bf553bbb13c559367b0f0171d590ede47899d01c521e29425ca592c0309a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220404"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

B2xIdentityUserFlow b2xIdentityUserFlow = new B2xIdentityUserFlow();
b2xIdentityUserFlow.id = "Partner";
b2xIdentityUserFlow.userFlowType = UserFlowType.SIGN_UP_OR_SIGN_IN;
b2xIdentityUserFlow.userFlowTypeVersion = 1;
LinkedList<IdentityProvider> identityProvidersList = new LinkedList<IdentityProvider>();
IdentityProvider identityProviders = new IdentityProvider();
identityProviders.id = "Facebook-OAuth";
identityProviders.type = "Facebook";
identityProviders.name = "Facebook";
identityProvidersList.add(identityProviders);
IdentityProviderCollectionResponse identityProviderCollectionResponse = new IdentityProviderCollectionResponse();
identityProviderCollectionResponse.value = identityProvidersList;
IdentityProviderCollectionPage identityProviderCollectionPage = new IdentityProviderCollectionPage(identityProviderCollectionResponse, null);
b2xIdentityUserFlow.identityProviders = identityProviderCollectionPage;

graphClient.identity().b2xUserFlows()
    .buildRequest()
    .post(b2xIdentityUserFlow);

```