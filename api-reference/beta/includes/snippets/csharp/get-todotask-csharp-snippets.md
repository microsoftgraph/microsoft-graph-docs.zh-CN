---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 24fa832be78cec7015af00094ed16d63b10f90dd
ms.sourcegitcommit: ef47b165f7a140cfc0309a275cb8722dd265660d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2020
ms.locfileid: "46873178"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tasks = await graphClient.Me.Todo.Lists.35e2-35e2-721a-e235-1a72e2351a7.Tasks
    .Request()
    .GetAsync();

```