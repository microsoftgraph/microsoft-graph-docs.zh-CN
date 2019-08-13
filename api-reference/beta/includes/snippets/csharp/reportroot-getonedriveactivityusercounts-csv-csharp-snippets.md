---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a482f80859d50b2736d9618afb47bbd5dfa617be
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36360049"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getOneDriveActivityUserCounts = await graphClient.Reports
    .GetOneDriveActivityUserCounts("D7")
    .Request()
    .GetAsync();

```