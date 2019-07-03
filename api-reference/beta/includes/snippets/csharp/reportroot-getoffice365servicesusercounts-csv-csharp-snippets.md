---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a80f100adcf65736815703c425d1eeab72f67027
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35520523"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getOffice365ServicesUserCounts = await graphClient.Reports.GetOffice365ServicesUserCounts('D7')
    .Request()
    .GetAsync();

```