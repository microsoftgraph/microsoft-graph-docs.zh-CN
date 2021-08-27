---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e54694618248cf32a2a7b9a2aa60c67513bf30798b1c1bbd3816c2b7d8bfd729
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106949"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ChatMessage chatMessage = new ChatMessage();
chatMessage.subject = null;
ItemBody body = new ItemBody();
body.contentType = BodyType.HTML;
body.content = "<attachment id=\"74d20c7f34aa4a7fb74e2b30004247c5\"></attachment>";
chatMessage.body = body;
LinkedList<ChatMessageAttachment> attachmentsList = new LinkedList<ChatMessageAttachment>();
ChatMessageAttachment attachments = new ChatMessageAttachment();
attachments.id = "74d20c7f34aa4a7fb74e2b30004247c5";
attachments.contentType = "application/vnd.microsoft.card.thumbnail";
attachments.contentUrl = null;
attachments.content = "{\r\n  \"title\": \"This is an example of posting a card\",\r\n  \"subtitle\": \"<h3>This is the subtitle</h3>\",\r\n  \"text\": \"Here is some body text. <br>\\r\\nAnd a <a href=\\\"http://microsoft.com/\\\">hyperlink</a>. <br>\\r\\nAnd below that is some buttons:\",\r\n  \"buttons\": [\r\n    {\r\n      \"type\": \"messageBack\",\r\n      \"title\": \"Login to FakeBot\",\r\n      \"text\": \"login\",\r\n      \"displayText\": \"login\",\r\n      \"value\": \"login\"\r\n    }\r\n  ]\r\n}";
attachments.name = null;
attachments.thumbnailUrl = null;
attachmentsList.add(attachments);
chatMessage.attachments = attachmentsList;

graphClient.teams("fbe2bf47-16c8-47cf-b4a5-4b9b187c508b").channels("19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2").messages()
    .buildRequest()
    .post(chatMessage);

```