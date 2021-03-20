---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 971e25762ce61b825d65a80145bf7e3510867ef8
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50971951"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ReferenceAttachment attachment = new ReferenceAttachment();
attachment.name = "Personal pictures";
attachment.sourceUrl = "https://contoso.com/personal/mario_contoso_net/Documents/Pics";
attachment.providerType = ReferenceAttachmentProvider.ONE_DRIVE_CONSUMER;
attachment.permission = ReferenceAttachmentPermission.EDIT;
attachment.isFolder = false;

graphClient.me().events("AAMkAGE1M88AADUv0uAAAG=").attachments()
    .buildRequest()
    .post(attachment);

```