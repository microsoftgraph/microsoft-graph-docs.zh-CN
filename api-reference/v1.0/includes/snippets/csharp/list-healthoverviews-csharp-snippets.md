---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8946ec18d3f18afced35bff1b4ff4a16a46bece1
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58259105"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var healthOverviews = await graphClient.Admin.ServiceAnnouncement.HealthOverviews
    .Request()
    .GetAsync();

```