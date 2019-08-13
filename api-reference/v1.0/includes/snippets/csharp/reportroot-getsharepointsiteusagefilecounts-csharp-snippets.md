---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 1ffff0f83acf0370ac8c8b14ada9a112267e1630
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36321772"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetSharePointSiteUsageFileCounts("D7")
    .Request()
    .GetAsync();

```