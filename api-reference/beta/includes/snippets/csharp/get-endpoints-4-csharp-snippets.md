---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 270187532274fe649df58c3b5ebf4c4fe90b1e7bb2dd678e677fde914766f1d8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54274899"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var dailyPrintUsageByUser = await graphClient.Print.Reports.DailyPrintUsageByUser
    .Request()
    .GetAsync();

```