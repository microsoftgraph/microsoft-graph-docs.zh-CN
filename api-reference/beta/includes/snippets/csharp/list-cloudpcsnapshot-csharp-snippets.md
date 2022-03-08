---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2647bb5289e3c7430fb5a685ef39188eb3792b17
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63335351"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var snapshots = await graphClient.DeviceManagement.VirtualEndpoint.Snapshots
    .Request()
    .GetAsync();

```