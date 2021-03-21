---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3f02076eda741be4cf3067099046f908179d01d2
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50982370"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AttachmentItem attachmentItem = new AttachmentItem();
attachmentItem.attachmentType = AttachmentType.FILE;
attachmentItem.name = "flower";
attachmentItem.size = 3483322L;

graphClient.me().messages("AAMkADI5MAAIT3drCAAA=").attachments()
    .createUploadSession(AttachmentCreateUploadSessionParameterSet
        .newBuilder()
        .withAttachmentItem(attachmentItem)
        .build())
    .buildRequest()
    .post();

```