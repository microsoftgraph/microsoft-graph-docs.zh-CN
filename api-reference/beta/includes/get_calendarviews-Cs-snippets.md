---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 587dcca493c5d5902e8a785803b67d2aabc0380f
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34473391"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var calendarView = await graphClient.Groups["02bd9fd6-8f93-4758-87c3-1fb73740a315"].CalendarView
    .Request()
    .Header("Prefer","outlook.body-content-type=\"text\"")
    .GetAsync();

```