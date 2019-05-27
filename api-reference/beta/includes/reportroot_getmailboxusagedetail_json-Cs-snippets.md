---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 89658912c0db797e2c89fb318ba8465b1629b241
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34442051"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getMailboxUsageDetail = await graphClient.Reports.GetMailboxUsageDetail('D7')
    .Request()
    .GetAsync();

```