---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9ae0ac0550291dd4894a2a808c7d7450ebc4436d85e85f14a0ec312562ebc334
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274343"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

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
    .reply(ConversationThreadReplyParameterSet
        .newBuilder()
        .withPost(post)
        .build())
    .buildRequest()
    .post();

```