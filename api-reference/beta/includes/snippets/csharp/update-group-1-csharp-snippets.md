---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3b69c2a597b58ca047726eec1af11b4be3d322a3
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50944230"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var group = new Group
{
    Description = "description-value",
    DisplayName = "displayName-value"
};

await graphClient.Groups["{group-id}"]
    .Request()
    .UpdateAsync(group);

```