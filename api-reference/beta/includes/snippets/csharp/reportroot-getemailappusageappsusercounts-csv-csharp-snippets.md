---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 263366d8fd69feff7899d18e50a3dca6bbf58f6b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36308589"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getEmailAppUsageAppsUserCounts = await graphClient.Reports
    .GetEmailAppUsageAppsUserCounts("D7")
    .Request()
    .GetAsync();

```