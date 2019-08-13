---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b5fb07fcc5624ce8c1f5befad0af4e6425bb84ea
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36307420"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"]
    .Range("A1:B2")
    .Request()
    .GetAsync();

```