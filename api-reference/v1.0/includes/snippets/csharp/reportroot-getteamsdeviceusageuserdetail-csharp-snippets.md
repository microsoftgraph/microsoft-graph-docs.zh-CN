---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 353d0e9efa8e61b17cba71bcd4cc1578695f1c1c
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35738093"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports.GetTeamsDeviceUsageUserDetail('D7')
    .Request()
    .GetAsync();

```