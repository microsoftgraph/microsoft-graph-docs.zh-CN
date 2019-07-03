---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 53bb91fe6b0ef4c7f2690e7879063bc040a37117
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35479707"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getTeamsUserActivityCounts = await graphClient.Reports.GetTeamsUserActivityCounts('D7')
    .Request()
    .GetAsync();

```