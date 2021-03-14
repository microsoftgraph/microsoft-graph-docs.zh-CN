---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 46bbc81cf569189656467d99da4cf98f264b40ec
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50799861"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var index = 5;

var values = JToken.Parse("[[1,2,3],[4,5,6]]");

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Tables["{workbookTable-id}"].Rows
    .Add(index,values)
    .Request()
    .PostAsync();

```