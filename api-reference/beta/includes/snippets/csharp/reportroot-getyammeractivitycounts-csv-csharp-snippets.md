---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 1dcacca897ea1a976df260c7ceb374c9f0b57ae9
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36358668"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getYammerActivityCounts = await graphClient.Reports
    .GetYammerActivityCounts("D7")
    .Request()
    .GetAsync();

```