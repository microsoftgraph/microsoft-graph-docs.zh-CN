---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2cc0fc886e860803224689a560582ffa6b9d7acab87e5139074df1db6924bdff
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219982"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ChatMessage chatMessage = new ChatMessage();
ItemBody body = new ItemBody();
body.content = "Hello world";
chatMessage.body = body;

graphClient.chats("19:2da4c29f6d7041eca70b638b43d45437@thread.v2").messages()
    .buildRequest()
    .post(chatMessage);

```