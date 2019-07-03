---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 42db3e856b46a6d1c6deef730695d1847ebc77b2
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35493693"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var events = await graphClient.Groups["02bd9fd6-8f93-4758-87c3-1fb73740a315"].Events
    .Request()
    .GetAsync();

```