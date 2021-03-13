---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1be149ebc5c5bc3e6f5a2ede550ed4d4e8aeea41
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50796911"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Drive.Root.Workbook.Worksheets["{workbookWorksheet-id}"]
    .Range()
    .ColumnsAfter(2)
    .Request()
    .GetAsync();

```