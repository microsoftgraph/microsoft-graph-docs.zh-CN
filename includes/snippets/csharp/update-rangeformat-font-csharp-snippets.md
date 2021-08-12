---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9e8ecc7b63484ed1bd411d5bd9f4ffd9d4f7a1ce24c3e335cf35ce53f26ad474
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54237702"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRangeFont = new WorkbookRangeFont
{
    Bold = true,
    Color = "#4B180E",
    Size = 26
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["Sheet1"]
    .Range("$A$1").Format.Font
    .Request()
    .UpdateAsync(workbookRangeFont);

```