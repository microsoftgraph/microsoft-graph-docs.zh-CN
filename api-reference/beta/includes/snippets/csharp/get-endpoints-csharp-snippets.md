---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 63278b5707a5bfab87a605ad73c8892b7a40958d
ms.sourcegitcommit: 6ec748ef00d025ee216274a608291be3c1257777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/27/2021
ms.locfileid: "50015386"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var reportRoot = await graphClient.Print.Reports["dailyPrintUsageSummariesByPrinter"]
    .Request()
    .GetAsync();

```