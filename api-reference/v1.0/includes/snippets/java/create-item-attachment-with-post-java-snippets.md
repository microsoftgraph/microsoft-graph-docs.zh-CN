---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1681f5e74ff3954d93577d2d54b38091414d5f4e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50983962"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Post post = new Post();
ItemBody body = new ItemBody();
body.contentType = BodyType.TEXT;
body.content = "I attached an event.";
post.body = body;
LinkedList<Attachment> attachmentsList = new LinkedList<Attachment>();
ItemAttachment attachments = new ItemAttachment();
attachments.name = "Holiday event";
Event item = new Event();
item.subject = "Discuss gifts for children";
ItemBody body1 = new ItemBody();
body1.contentType = BodyType.HTML;
body1.content = "Let's look for funding!";
item.body = body1;
DateTimeTimeZone start = new DateTimeTimeZone();
start.dateTime = "2019-12-02T18:00:00";
start.timeZone = "Pacific Standard Time";
item.start = start;
DateTimeTimeZone end = new DateTimeTimeZone();
end.dateTime = "2019-12-02T19:00:00";
end.timeZone = "Pacific Standard Time";
item.end = end;
attachments.item = item;
attachmentsList.add(attachments);
AttachmentCollectionResponse attachmentCollectionResponse = new AttachmentCollectionResponse();
attachmentCollectionResponse.value = attachmentsList;
AttachmentCollectionPage attachmentCollectionPage = new AttachmentCollectionPage(attachmentCollectionResponse, null);
post.attachments = attachmentCollectionPage;

graphClient.groups("1848753d-185d-4c08-a4e4-6ee40521d115").threads("AAQkADJUdfolA==")
    .reply(ConversationThreadReplyParameterSet
        .newBuilder()
        .withPost(post)
        .build())
    .buildRequest()
    .post();

```