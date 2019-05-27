---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9e0b0da591a23ec7b262dfc5ea4529a1404ede1b
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34447591"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plannerTaskDetails = await graphClient.Planner.Tasks["gcrYAaAkgU2EQUvpkNNXLGQAGTtu"].Details
    .Request()
    .GetAsync();

```