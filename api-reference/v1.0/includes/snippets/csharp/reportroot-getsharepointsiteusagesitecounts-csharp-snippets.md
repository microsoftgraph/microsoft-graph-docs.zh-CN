---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 1a2cf3bb918cb06a8313b136ba3de1292cc2a0a6
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36357971"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetSharePointSiteUsageSiteCounts("D7")
    .Request()
    .GetAsync();

```