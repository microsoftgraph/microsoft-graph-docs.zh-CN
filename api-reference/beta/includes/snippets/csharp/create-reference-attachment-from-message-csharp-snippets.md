---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fab33ecaf54f0dc630088a242556243d6c4ba5c7ebf122a4f79950f482923381
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56904036"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var attachment = new ReferenceAttachment
{
    Name = "Personal pictures",
    SourceUrl = "https://contoso.com/personal/mario_contoso_net/Documents/Pics",
    ProviderType = ReferenceAttachmentProvider.OneDriveConsumer,
    Permission = ReferenceAttachmentPermission.Edit,
    IsFolder = true
};

await graphClient.Me.Messages["{message-id}"].Attachments
    .Request()
    .AddAsync(attachment);

```