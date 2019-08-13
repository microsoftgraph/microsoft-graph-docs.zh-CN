---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 01bcdf7cab53c51f9935d74c352325c1c4e71c89
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36360095"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getOneDriveUsageAccountCounts = await graphClient.Reports
    .GetOneDriveUsageAccountCounts("D7")
    .Request()
    .GetAsync();

```