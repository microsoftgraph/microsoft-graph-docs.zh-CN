---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 29f44c64f4f6b9fab9403c37dd8ea4746adf0fe9
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2020
ms.locfileid: "44052429"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var attachmentItem = new AttachmentItem
{
    AttachmentType = AttachmentType.File,
    Name = "flower",
    Size = 3483322
};

await graphClient.Me.Events["AAMkADU5CCmSAAA="].Attachments
    .CreateUploadSession(attachmentItem)
    .Request()
    .PostAsync();

```