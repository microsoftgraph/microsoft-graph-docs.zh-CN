---
description: 自动生成的文件。 不修改
ms.openlocfilehash: d9facff7b4adc71e3fdc1e15c11026fc9cdc5208
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36308800"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getEmailActivityCounts = await graphClient.Reports
    .GetEmailActivityCounts("D7")
    .Request()
    .GetAsync();

```