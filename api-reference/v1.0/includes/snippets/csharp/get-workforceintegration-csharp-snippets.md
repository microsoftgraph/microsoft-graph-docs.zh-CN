---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7274f06fcd816db0da48be70cf6fa6a46bb63d86
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2020
ms.locfileid: "44217013"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workforceIntegration = await graphClient.Teamwork.WorkforceIntegrations["{workforceintegrationid}"]
    .Request()
    .GetAsync();

```