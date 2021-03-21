---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4b62ef8f4ab7442fc9eb10199fae20af8ce7fca9
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50959555"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var monthlyPrintUsageByUser = await graphClient.Reports.MonthlyPrintUsageByUser
    .Request()
    .GetAsync();

```