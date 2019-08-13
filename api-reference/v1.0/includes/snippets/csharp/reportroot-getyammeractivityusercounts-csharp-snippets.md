---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 402406310b6ff9d2b6199b58eee620440c37d59e
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36320346"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetYammerActivityUserCounts("D7")
    .Request()
    .GetAsync();

```