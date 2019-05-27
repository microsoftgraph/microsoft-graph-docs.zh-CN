---
description: 自动生成的文件。 不修改
ms.openlocfilehash: dd62d3ed08df707bb815c5c10c2dd81f13076f00
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34465062"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports.GetMailboxUsageStorage('D7')
    .Request()
    .GetAsync();

```