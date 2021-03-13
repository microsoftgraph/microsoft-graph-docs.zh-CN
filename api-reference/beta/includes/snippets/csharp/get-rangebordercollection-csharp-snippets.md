---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 17cb4a1f6879312017b4b443e8bed37e4f896e0c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50786708"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var borders = await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Names["{workbookNamedItem-id}"]
    .Range().Format.Borders
    .Request()
    .GetAsync();

```