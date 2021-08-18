---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9167d787b6f8727914fe609a1288dc237452ca53b6219fb3aca4591504fa40f0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163169"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ChatMessageHostedContentCollectionPage hostedContents = graphClient.chats("19:2da4c29f6d7041eca70b638b43d45437@thread.v2").messages("1615971548136").hostedContents()
    .buildRequest()
    .get();

```