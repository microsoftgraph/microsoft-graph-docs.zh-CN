---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a1c74012197d9ae10843ef0a0dd4d1fb8d67e1fa628b4d3275e83d01f4e9b134
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409649"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var rows = await graphClient.Me.Drive.Root.Workbook.Worksheets["{workbookWorksheet-id}"]
    .Range("A1:Z10")
    .VisibleView().Rows
    .Request()
    .GetAsync();

```