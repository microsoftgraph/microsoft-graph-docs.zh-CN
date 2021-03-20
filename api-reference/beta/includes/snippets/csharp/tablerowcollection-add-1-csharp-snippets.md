---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c149dd4b6dac1ab8292d30cdffd26e15ce6d11c0
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50952886"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var values = JToken.Parse("[[1,2,3],[4,5,6]]");

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Tables["{workbookTable-id}"].Rows
    .Add(null,values)
    .Request()
    .PostAsync();

```