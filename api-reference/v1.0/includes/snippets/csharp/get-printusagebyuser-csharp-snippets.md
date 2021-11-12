---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f5ccca509dd02a6c0ee286543bc984e42126de3356c4f3b562c7202ca8da065d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104941"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printUsageByUser = await graphClient.Reports.DailyPrintUsageByUser["{printUsageByUser-id}"]
    .Request()
    .GetAsync();

```