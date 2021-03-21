---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e800d83d29540650d10a306b830dfa9a84f3e89e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50954817"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var dailyPrintUsageByUser = await graphClient.Reports.DailyPrintUsageByUser
    .Request()
    .GetAsync();

```