---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6f65a45882d05626ce9c7fef002b9a1cc3354f88
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "52474732"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var roleScheduleInstances = await graphClient.RoleManagement.Directory
    .RoleScheduleInstances("parameterValue","parameterValue","parameterValue","parameterValue")
    .Request()
    .GetAsync();

```