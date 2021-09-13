---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e85e96aee2a15ed2419ad52ddbe6d8fa8db149e32391585bdd6d00beb0489e7f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161962"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Root.Workbook.Worksheets["{workbookWorksheet-id}"]
    .Range()
    .RowsAbove()
    .Request()
    .GetAsync();

```