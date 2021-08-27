---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 66568f9c37762c9eba21fc4d4c96ca1a6417db87ac43bbb660401e28898f486a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333236"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ChatMessage chatMessage = new ChatMessage();
chatMessage.createdDateTime = OffsetDateTimeSerializer.deserialize("2019-02-04T19:58:15.511Z");
ChatMessageFromIdentitySet from = new ChatMessageFromIdentitySet();
Identity user = new Identity();
user.id = "8c0a1a67-50ce-4114-bb6c-da9c5dbcf6ca";
user.displayName = "John Doe";
from.user = user;
chatMessage.from = from;
ItemBody body = new ItemBody();
body.contentType = BodyType.HTML;
body.content = "Hello World";
chatMessage.body = body;

graphClient.teams("57fb72d0-d811-46f4-8947-305e6072eaa5").channels("19:4b6bed8d24574f6a9e436813cb2617d8@thread.tacv2").messages("1590776551682").replies()
    .buildRequest()
    .post(chatMessage);

```