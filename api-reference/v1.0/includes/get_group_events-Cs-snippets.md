---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 42db3e856b46a6d1c6deef730695d1847ebc77b2
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34452428"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var events = await graphClient.Groups["02bd9fd6-8f93-4758-87c3-1fb73740a315"].Events
    .Request()
    .GetAsync();

```