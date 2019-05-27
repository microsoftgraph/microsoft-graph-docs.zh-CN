---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 978a914a223171b4cdb360eaced84e7d1bf959fd
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34441554"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getOffice365GroupsActivityCounts = await graphClient.Reports.GetOffice365GroupsActivityCounts('D7')
    .Request()
    .GetAsync();

```