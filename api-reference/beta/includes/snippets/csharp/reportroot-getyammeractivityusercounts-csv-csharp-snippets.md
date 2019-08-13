---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 1639775c575ff219aa158b22c8783886082bfa87
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36358633"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getYammerActivityUserCounts = await graphClient.Reports
    .GetYammerActivityUserCounts("D7")
    .Request()
    .GetAsync();

```