---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b55e7f7a795b2cf7bdfd85b0c7bbd4fbacd3c68e3c4db25453ef0d6622c9702b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54274684"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var dailyPrintUsageByPrinter = await graphClient.Print.Reports.DailyPrintUsageByPrinter
    .Request()
    .GetAsync();

```