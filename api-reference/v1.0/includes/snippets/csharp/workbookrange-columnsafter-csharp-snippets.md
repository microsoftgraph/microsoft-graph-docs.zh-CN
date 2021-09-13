---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1a877d8453b7d94e557435ad17c580f8324f188722bdd3d438e06df8282bce07
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279299"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Root.Workbook.Worksheets["{workbookWorksheet-id}"]
    .Range()
    .ColumnsAfter(2)
    .Request()
    .GetAsync();

```