---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2404755656cf49245f4c20180d6979628c73fe9016cbd0d10f5dd040edd3933d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57334147"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ChatMessage chatMessage = new ChatMessage();
ItemBody body = new ItemBody();
body.contentType = BodyType.HTML;
body.content = "Here's the latest budget. <attachment id=\"153fa47d-18c9-4179-be08-9879815a9f90\"></attachment>";
chatMessage.body = body;
LinkedList<ChatMessageAttachment> attachmentsList = new LinkedList<ChatMessageAttachment>();
ChatMessageAttachment attachments = new ChatMessageAttachment();
attachments.id = "153fa47d-18c9-4179-be08-9879815a9f90";
attachments.contentType = "reference";
attachments.contentUrl = "https://m365x987948.sharepoint.com/sites/test/Shared%20Documents/General/test%20doc.docx";
attachments.name = "Budget.docx";
attachmentsList.add(attachments);
chatMessage.attachments = attachmentsList;

graphClient.teams("fbe2bf47-16c8-47cf-b4a5-4b9b187c508b").channels("19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2").messages()
    .buildRequest()
    .post(chatMessage);

```