---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 3a15085eb4a155e09ad6974909cef1ea157a8070
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36358870"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getTeamsDeviceUsageDistributionUserCounts = await graphClient.Reports
    .GetTeamsDeviceUsageDistributionUserCounts("D7")
    .Request()
    .GetAsync();

```