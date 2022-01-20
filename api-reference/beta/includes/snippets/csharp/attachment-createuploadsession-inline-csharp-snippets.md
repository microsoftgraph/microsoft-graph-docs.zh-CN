---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4adf10581c7518451fe3812df21cac55b9a7f1d3
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62107095"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var attachmentItem = new AttachmentItem
{
    AttachmentType = AttachmentType.File,
    Name = "scenary",
    Size = 7208534,
    IsInline = true,
    ContentId = "my_inline_picture"
};

await graphClient.Me.Messages["{message-id}"].Attachments
    .CreateUploadSession(attachmentItem)
    .Request()
    .PostAsync();

```