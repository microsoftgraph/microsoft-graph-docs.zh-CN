---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9c65a0ce0fb110ebdc4c611a012adb05564d80cd
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35855568"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetTeamsDeviceUsageUserDetail('D7')
    .Request()
    .GetAsync();

```