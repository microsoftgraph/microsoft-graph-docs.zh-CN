---
description: 自动生成的文件。 不修改
ms.openlocfilehash: eaaa002278b2b7e45e9bf60b35e634a0624dd4de
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35736712"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRangeFill = new WorkbookRangeFill
{
    Color = "color-value"
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"].Range().Format.Fill
    .Request()
    .UpdateAsync(workbookRangeFill);

```