---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 46bbc81cf569189656467d99da4cf98f264b40ec
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50941447"
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