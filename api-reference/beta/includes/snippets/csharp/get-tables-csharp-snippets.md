---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3d47c1f0fc187617424d68c05305bcd99b00b22a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50805413"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tables = await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Tables
    .Request()
    .GetAsync();

```