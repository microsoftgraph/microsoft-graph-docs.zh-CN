---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8d47e6d6915ec9d4a122bb76cff724911528cccd
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/29/2021
ms.locfileid: "59996521"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getAttackSimulationRepeatOffenders = await graphClient.Reports
    .GetAttackSimulationRepeatOffenders()
    .Request()
    .GetAsync();

```