---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 4749c2ac9827b238b7827558057fe468f721d3f9
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35467123"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports.GetEmailAppUsageVersionsUserCounts('D7')
    .Request()
    .GetAsync();

```