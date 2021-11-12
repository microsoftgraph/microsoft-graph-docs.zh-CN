---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 02cb0f5b3a2ad8f2e8bfaaf6430f0f68a67721536c7c5509508703a50950b236
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221285"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var rows = await graphClient.Drive.Root.Workbook.Worksheets["{workbookWorksheet-id}"]
    .Range("A1:Z10")
    .VisibleView().Rows
    .Request()
    .GetAsync();

```