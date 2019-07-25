---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a788605687ac183daaa0bc49ad6f13742179dda5
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35872286"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getSkypeForBusinessDeviceUsageUserCounts = await graphClient.Reports
    .GetSkypeForBusinessDeviceUsageUserCounts('D7')
    .Request()
    .GetAsync();

```