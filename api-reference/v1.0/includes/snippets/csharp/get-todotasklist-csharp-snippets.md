---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3fff492319c44280acce3d579630d9d2213d3bf6
ms.sourcegitcommit: 6ec748ef00d025ee216274a608291be3c1257777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/27/2021
ms.locfileid: "50015832"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var lists = await graphClient.Me.Todo.Lists
    .Request()
    .GetAsync();

```