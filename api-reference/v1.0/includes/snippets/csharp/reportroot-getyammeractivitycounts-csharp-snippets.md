---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 8d97904f7dade188938e4269829c3a6f2a242340
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36320392"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetYammerActivityCounts("D7")
    .Request()
    .GetAsync();

```