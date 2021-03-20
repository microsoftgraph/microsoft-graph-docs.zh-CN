---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d5afb859b7d2c680e1a4692d45441742d78d4e64
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50961544"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plans = await graphClient.Planner.Rosters["{plannerRoster-id}"].Plans
    .Request()
    .GetAsync();

```