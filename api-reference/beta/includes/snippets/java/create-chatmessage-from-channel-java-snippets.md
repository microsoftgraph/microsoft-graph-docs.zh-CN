---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 08ee2584476c76ba8a4915042395963db635a72d
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35864399"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

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

graphClient.teams("{id}").channels("{id}").messages()
    .buildRequest()
    .post(chatMessage);

```