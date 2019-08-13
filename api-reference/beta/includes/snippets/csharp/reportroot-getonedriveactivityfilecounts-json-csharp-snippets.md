---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 08e2aed57b0589d0e71aa68dd6955aeb519ee017
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36360222"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getOneDriveActivityFileCounts = await graphClient.Reports
    .GetOneDriveActivityFileCounts("D7")
    .Request()
    .GetAsync();

```