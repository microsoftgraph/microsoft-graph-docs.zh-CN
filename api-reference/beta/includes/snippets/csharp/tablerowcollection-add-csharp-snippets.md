---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3bdcaa7d428439e0b1f73c90a8e0c842e0036736
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2021
ms.locfileid: "49945828"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var values = JToken.Parse("[[1,2,3],[4,5,6]]");

await graphClient.Me.Drive.Items["{id}"].Workbook.Tables["{id|name}"].Rows
    .Add(null,values)
    .Request()
    .PostAsync();

```