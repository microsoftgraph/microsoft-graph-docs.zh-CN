---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dd1b8d0d850f4e9e5f1a3439cb59382f5651e6b9
ms.sourcegitcommit: d8a425766aa6a56027b8576bbec6a9d1ae3e079c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/21/2019
ms.locfileid: "37544220"
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
attachments.providerType = "oneDriveConsumer";
attachments.permission = "Edit";
attachments.isFolder = "True";
attachmentsList.add(attachments);
post.attachments = attachmentsList;

graphClient.groups("1848753d-185d-4c08-a4e4-6ee40521d115").threads("AAQkADJUdfolA==")
    .reply(post)
    .buildRequest()
    .post();

```