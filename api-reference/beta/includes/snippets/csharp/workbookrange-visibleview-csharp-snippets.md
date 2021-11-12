---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0ddb5e523f185259c2645a04060f8d8ed46738e1c9cd9a2a201a29f9e436cfd1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105464"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRangeView = await graphClient.Drive.Root.Workbook.Worksheets["{workbookWorksheet-id}"]
    .Range("A1:Z10")
    .VisibleView()
    .Request()
    .GetAsync();

```