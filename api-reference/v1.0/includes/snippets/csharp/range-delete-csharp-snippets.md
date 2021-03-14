---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 78c0fcc4fec7e469a8a66177d45823d12081dfba
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50778759"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var shift = "shift-value";

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Names["{workbookNamedItem-id}"]
    .Range()
    .Delete(shift)
    .Request()
    .PostAsync();

```