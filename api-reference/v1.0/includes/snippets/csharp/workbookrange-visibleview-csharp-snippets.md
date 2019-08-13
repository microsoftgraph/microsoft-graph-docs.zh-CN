---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 79f86b0aae3b55ae1b20ea8c57f8c6d08ce1ec51
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36307784"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRangeView = await graphClient.Me.Drive.Root.Workbook.Worksheets["{id}"]
    .Range("A1:Z10")
    .VisibleView()
    .Request()
    .GetAsync();

```