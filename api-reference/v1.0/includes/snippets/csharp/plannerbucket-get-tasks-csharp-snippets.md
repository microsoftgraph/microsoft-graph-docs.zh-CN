---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3fffc41c99db18e1f4205c58287b1850d6788e9e
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "37637861"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tasks = await graphClient.Planner.Buckets["{task-id}"].Tasks
    .Request()
    .GetAsync();

```