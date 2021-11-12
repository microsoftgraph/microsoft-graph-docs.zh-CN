---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dff5b34bf1ac06765171a5006c45aa59f4aae8c2b472cd3434b561816f1788a3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333449"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printUsageByUser = await graphClient.Print.Reports.DailyPrintUsageByUser["{printUsageByUser-id}"]
    .Request()
    .GetAsync();

```