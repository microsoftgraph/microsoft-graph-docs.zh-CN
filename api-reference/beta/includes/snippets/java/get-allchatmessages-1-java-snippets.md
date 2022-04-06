---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 702a259b36816995db21d0c98c9f6397fa0e52fb
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2022
ms.locfileid: "63759164"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ChatMessageCollectionPage messages = graphClient.chats("19:2da4c29f6d7041eca70b638b43d45437@thread.v2").messages()
    .buildRequest()
    .orderBy("createdDateTime desc")
    .top(2)
    .get();

```