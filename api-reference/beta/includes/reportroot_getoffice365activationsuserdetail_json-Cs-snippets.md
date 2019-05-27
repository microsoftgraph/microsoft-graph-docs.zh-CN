---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 3db8faa109bad7b434875d178f14a999fdbe40e3
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34441792"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getOffice365ActivationsUserDetail = await graphClient.Reports.GetOffice365ActivationsUserDetail()
    .Request()
    .GetAsync();

```