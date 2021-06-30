---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0e2e2242c6396add51bb688aa1a4fd0c2e1b0746
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53210750"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var serviceHealth = await graphClient.Admin.ServiceAnnouncement.HealthOverviews["{serviceHealth-id}"]
    .Request()
    .GetAsync();

```