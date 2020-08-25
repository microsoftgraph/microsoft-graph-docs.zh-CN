---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 88897d1a184fbb22552110b15c6a3a165fb309e8
ms.sourcegitcommit: ef47b165f7a140cfc0309a275cb8722dd265660d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2020
ms.locfileid: "46873051"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var linkedResources = await graphClient.Me.Todo.Lists.Dfsdc-f9dfdfs-dcsda9.Tasks.E2dc-f9cce2-dce29.LinkedResources
    .Request()
    .GetAsync();

```