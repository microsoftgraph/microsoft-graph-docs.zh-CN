---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 7fe62dc0d8c5af605bebb111f9258b553a91a91c
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35871760"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getTeamsDeviceUsageUserDetail = await graphClient.Reports
    .GetTeamsDeviceUsageUserDetail('D7')
    .Request()
    .GetAsync();

```