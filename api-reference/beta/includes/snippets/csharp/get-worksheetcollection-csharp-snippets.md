---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 42f11b04ce9b3cf36b9351c006f306f2b202cbb0
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50803056"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var worksheets = await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Worksheets
    .Request()
    .GetAsync();

```