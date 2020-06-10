---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bc4a360815d5cd0cad8320b368dcb7bb626de807
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44684275"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var index = null;

var values = JToken.Parse("[[1,2,3],[4,5,6]]");

await graphClient.Me.Drive.Items["{id}"].Workbook.Tables["{id|name}"].Rows
    .Add(index,values)
    .Request()
    .PostAsync();

```