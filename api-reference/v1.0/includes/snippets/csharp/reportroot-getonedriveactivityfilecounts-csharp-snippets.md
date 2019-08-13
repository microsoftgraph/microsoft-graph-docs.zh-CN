---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 563d380b7164d54749dadb637bdd200e0278a061
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36373973"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetOneDriveActivityFileCounts("D7")
    .Request()
    .GetAsync();

```