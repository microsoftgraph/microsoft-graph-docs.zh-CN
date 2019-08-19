---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 59475759b867dd1937e5d6e5bb06a8324042d69c
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2019
ms.locfileid: "36460783"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var activityStatistics = await graphClient.Me.Analytics.ActivityStatistics
    .Request()
    .GetAsync();

```