---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 69bae08300d493551c300c9874df37e5efd19469
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62107091"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AttachmentItem attachmentItem = new AttachmentItem();
attachmentItem.attachmentType = AttachmentType.FILE;
attachmentItem.name = "scenary";
attachmentItem.size = 7208534L;
attachmentItem.isInline = true;
attachmentItem.contentId = "my_inline_picture";

graphClient.me().messages("AAMkAGUwNjQ4ZjIxLTQ3Y2YtNDViMi1iZjc4LTMA=").attachments()
    .createUploadSession(AttachmentCreateUploadSessionParameterSet
        .newBuilder()
        .withAttachmentItem(attachmentItem)
        .build())
    .buildRequest()
    .post();

```