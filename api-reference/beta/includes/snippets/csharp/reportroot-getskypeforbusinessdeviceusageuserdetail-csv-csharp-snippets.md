---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 1544f72fdfeb1567f02015dfbf4158d6f2a9d070
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35520403"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getSkypeForBusinessDeviceUsageUserDetail = await graphClient.Reports.GetSkypeForBusinessDeviceUsageUserDetail('D7')
    .Request()
    .GetAsync();

```