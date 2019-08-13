---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 32b78dc0e8ef57eb80edcffd8b863489b53b99d9
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36359842"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getSharePointActivityFileCounts = await graphClient.Reports
    .GetSharePointActivityFileCounts("D7")
    .Request()
    .GetAsync();

```