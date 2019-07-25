---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 8f07035f46080193ee4d549d16eb152782278470
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35865062"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var events = await graphClient.Me.Calendar.Events
    .Request()
    .GetAsync();

```