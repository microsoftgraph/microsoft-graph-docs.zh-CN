---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1d98a8d2fa93c4f9cc5034f032678f71f852e85e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50799938"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var driveItem = new DriveItem
{
    Name = "new-file-name.docx"
};

await graphClient.Me.Drive.Items["{driveItem-id}"]
    .Request()
    .UpdateAsync(driveItem);

```