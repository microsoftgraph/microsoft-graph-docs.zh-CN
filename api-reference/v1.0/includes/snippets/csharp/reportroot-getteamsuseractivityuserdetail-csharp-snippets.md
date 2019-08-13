---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 07391635084d5aeac4f21e91d49ae388ab60398b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36369417"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetTeamsUserActivityUserDetail("D7")
    .Request()
    .GetAsync();

```