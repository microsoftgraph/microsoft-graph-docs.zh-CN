---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6a52eb5906bcc98ea52ef06632abf123d7844268
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50787883"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var attachmentItem = new AttachmentItem
{
    AttachmentType = AttachmentType.File,
    Name = "flower",
    Size = 3483322
};

await graphClient.Me.Messages["{message-id}"].Attachments
    .CreateUploadSession(attachmentItem)
    .Request()
    .PostAsync();

```