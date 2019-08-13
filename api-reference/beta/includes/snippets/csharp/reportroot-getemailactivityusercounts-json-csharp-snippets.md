---
description: 自动生成的文件。 不修改
ms.openlocfilehash: dd8754004d13baaa4da8c85659d22a8cccc5405c
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36308641"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getEmailActivityUserCounts = await graphClient.Reports
    .GetEmailActivityUserCounts("D7")
    .Request()
    .GetAsync();

```