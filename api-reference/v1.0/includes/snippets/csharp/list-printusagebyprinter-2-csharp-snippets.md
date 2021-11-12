---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 58a9a79b0cfaf4fa2f2817ccdc467ef416a48af3c75bb61f15986bf83416652f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56831183"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var monthlyPrintUsageByPrinter = await graphClient.Reports.MonthlyPrintUsageByPrinter
    .Request()
    .GetAsync();

```