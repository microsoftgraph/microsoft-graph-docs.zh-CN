---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d6a8ec381d863d40d84cfbda0f9da2f49168d7b3
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50788274"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Names["{workbookNamedItem-id}"]
    .Range().Format
    .AutofitColumns()
    .Request()
    .PostAsync();

```