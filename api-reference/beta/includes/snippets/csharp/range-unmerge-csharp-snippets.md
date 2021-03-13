---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: acc1aa1de144d5ddd9f6ac54bb107f0ea973f397
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50799937"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Names["{workbookNamedItem-id}"]
    .Range()
    .Unmerge()
    .Request()
    .PostAsync();

```