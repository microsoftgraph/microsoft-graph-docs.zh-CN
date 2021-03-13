---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8ead91358a7d252e77dc439285e139e3461eba7f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50792428"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var rows = await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Tables["{workbookTable-id}"].Rows
    .Request()
    .Skip(5)
    .Top(5)
    .GetAsync();

```