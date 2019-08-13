---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 220aff5966eff57d65d19da520311ece9d5630d0
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36359508"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getSkypeForBusinessDeviceUsageDistributionUserCounts = await graphClient.Reports
    .GetSkypeForBusinessDeviceUsageDistributionUserCounts("D7")
    .Request()
    .GetAsync();

```