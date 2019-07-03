---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 6d71ad418eb9549c50a55c8b9c091ee8cbfbbffd
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35492959"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports.GetSharePointSiteUsageStorage('D7')
    .Request()
    .GetAsync();

```