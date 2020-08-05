---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9c6cdaebc0cbc72a511d39c089d82c140f4796e3
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46567065"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var itemInsightsSettings = new ItemInsightsSettings
{
    DisabledForGroup = "edbfe4fb-ec70-4300-928f-dbb2ae86c981"
};

await graphClient.Organization["{organizationId}"].Settings.ItemInsights
    .Request()
    .UpdateAsync(itemInsightsSettings);

```