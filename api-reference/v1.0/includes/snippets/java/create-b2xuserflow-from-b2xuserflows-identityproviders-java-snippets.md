---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 92e41a4fdd9ae24935fcf46ab93eabb8b2647a89
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51920284"
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