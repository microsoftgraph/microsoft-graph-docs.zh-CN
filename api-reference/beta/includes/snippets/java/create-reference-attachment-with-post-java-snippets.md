---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6d4784a7c1a286ef108ffbce0c93b4e74e8e74d1
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48982016"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Post post = new Post();
ItemBody body = new ItemBody();
body.contentType = BodyType.TEXT;
body.content = "I attached a reference to a file on OneDrive.";
post.body = body;
LinkedList<Attachment> attachmentsList = new LinkedList<Attachment>();
ReferenceAttachment attachments = new ReferenceAttachment();
attachments.name = "Personal pictures";
attachments.sourceUrl = "https://contoso.com/personal/mario_contoso_net/Documents/Pics";
attachments.providerType = ReferenceAttachmentProvider.ONE_DRIVE_CONSUMER;
attachments.permission = ReferenceAttachmentPermission.EDIT;
attachments.isFolder = false;
attachmentsList.add(attachments);
AttachmentCollectionResponse attachmentCollectionResponse = new AttachmentCollectionResponse();
attachmentCollectionResponse.value = attachmentsList;
AttachmentCollectionPage attachmentCollectionPage = new AttachmentCollectionPage(attachmentCollectionResponse, null);
post.attachments = attachmentCollectionPage;

graphClient.groups("1848753d-185d-4c08-a4e4-6ee40521d115").threads("AAQkADJUdfolA==")
    .reply(post)
    .buildRequest()
    .post();

```