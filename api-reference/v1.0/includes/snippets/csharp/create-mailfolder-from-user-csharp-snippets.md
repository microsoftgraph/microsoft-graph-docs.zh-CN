---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b5d6b0f12f66d1ffc78ec9207b63cf68772167a8
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/11/2020
ms.locfileid: "49661831"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var mailFolder = new MailFolder
{
    DisplayName = "Clutter"
};

await graphClient.Me.MailFolders
    .Request()
    .AddAsync(mailFolder);

```