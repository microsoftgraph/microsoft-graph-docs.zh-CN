---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4cf6f7f2c32e0ac976074a7156e11f6017b7725691b33bc332ff86ba6aeb3ce0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902918"
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