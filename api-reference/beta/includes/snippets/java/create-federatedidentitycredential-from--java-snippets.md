---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cf8c53cb960bfe9037b26109ebb09bc2a9fda366
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60689226"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

FederatedIdentityCredential federatedIdentityCredential = new FederatedIdentityCredential();
federatedIdentityCredential.name = "testing02";
federatedIdentityCredential.issuer = "https://login.microsoftonline.com/3d1e2be9-a10a-4a0c-8380-7ce190f98ed9/v2.0";
federatedIdentityCredential.subject = "a7d388c3-5e3f-4959-ac7d-786b3383006a";
LinkedList<String> audiencesList = new LinkedList<String>();
audiencesList.add("api://AzureADTokenExchange");
federatedIdentityCredential.audiences = audiencesList;

graphClient.applications("bcd7c908-1c4d-4d48-93ee-ff38349a75c8").federatedIdentityCredentials()
    .buildRequest()
    .post(federatedIdentityCredential);

```