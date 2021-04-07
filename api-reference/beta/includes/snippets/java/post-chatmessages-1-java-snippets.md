---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3ce9473d72faf65e58e777a493bc22b05bf08db3
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2021
ms.locfileid: "51610658"
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