---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7109766de40f02c35194ca208d299aa17c1b3b10eab49b3c431488afd6fdb3db
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274439"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var monthlyPrintUsageByUser = await graphClient.Reports.MonthlyPrintUsageByUser
    .Request()
    .GetAsync();

```