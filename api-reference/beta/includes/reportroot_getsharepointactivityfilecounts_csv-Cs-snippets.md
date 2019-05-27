---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9a33b75d4af415c149616f578f21ee7ea066e247
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34440826"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getSharePointActivityFileCounts = await graphClient.Reports.GetSharePointActivityFileCounts('D7')
    .Request()
    .GetAsync();

```