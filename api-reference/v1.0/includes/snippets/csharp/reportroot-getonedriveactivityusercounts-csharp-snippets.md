---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 218653f8e50fc7ba762d70e966df7494961e7808
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36373968"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetOneDriveActivityUserCounts("D7")
    .Request()
    .GetAsync();

```