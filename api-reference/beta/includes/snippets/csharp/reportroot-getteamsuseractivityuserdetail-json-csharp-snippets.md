---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 1580bf655c6720528cb776135e69d19a3133466c
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36358725"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getTeamsUserActivityUserDetail = await graphClient.Reports
    .GetTeamsUserActivityUserDetail("D7")
    .Request()
    .GetAsync();

```