---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 78a46a9c67007df96ec3324b66a5a85b5d6e65b4
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "37637948"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tasks = await graphClient.Planner.Tasks
    .Request()
    .GetAsync();

```