---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 04f7763e97ccd86f94f7c2bbb2977c6eae8fe8d2
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50803364"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Worksheets["{workbookWorksheet-id}"].Charts["{workbookChart-id}"].Format.Fill
    .Clear()
    .Request()
    .PostAsync();

```