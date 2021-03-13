---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c705533ae4b7aaa483e48eb7f205119c77276c5f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50780912"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printUsageByUser = await graphClient.Print.Reports.DailyPrintUsageSummariesByUser["{printUsageByUser-id}"]
    .Request()
    .GetAsync();

```