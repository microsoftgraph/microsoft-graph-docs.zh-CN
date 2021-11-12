---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 64ca44246a914183261c42ff14a78a476b99b0db6680cb13ddcab74b81ebf65c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163893"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var pivotTables = await graphClient.Drive.Root.Workbook.Worksheets["{workbookWorksheet-id}"].PivotTables
    .Request()
    .GetAsync();

```