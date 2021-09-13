---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5b63c87ec5029716d11a20f73f007e3195f311607242a081e82ee2bc56d529aa
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57164220"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Root.Workbook.Worksheets["{workbookWorksheet-id}"]
    .Range()
    .RowsBelow()
    .Request()
    .GetAsync();

```