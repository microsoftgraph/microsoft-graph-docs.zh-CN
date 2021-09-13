---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d8e765f6b6f8dd61db736b94f648c1387ca83f3a7c36906cb7454f9ad8066025
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278607"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ChatMessage chatMessage = new ChatMessage();
ItemBody body = new ItemBody();
body.contentType = BodyType.HTML;
body.content = "Hello World";
chatMessage.body = body;

graphClient.teams("57fb72d0-d811-46f4-8947-305e6072eaa5").channels("19:4b6bed8d24574f6a9e436813cb2617d8@thread.tacv2").messages("1590776551682").replies()
    .buildRequest()
    .post(chatMessage);

```