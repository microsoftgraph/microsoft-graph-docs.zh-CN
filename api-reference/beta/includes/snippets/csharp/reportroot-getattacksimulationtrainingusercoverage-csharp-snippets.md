---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ae01fe2d60d835c7b9ed7d5598a5036d9bc36be8
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/29/2021
ms.locfileid: "59997192"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getAttackSimulationTrainingUserCoverage = await graphClient.Reports
    .GetAttackSimulationTrainingUserCoverage()
    .Request()
    .GetAsync();

```