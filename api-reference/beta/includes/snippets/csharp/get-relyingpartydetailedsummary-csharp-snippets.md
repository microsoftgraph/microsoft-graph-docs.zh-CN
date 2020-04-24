---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f154e413a4a479aee3024572fe93f197f5a662f7
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43806146"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getRelyingPartyDetailedSummary = await graphClient.Reports
    .GetRelyingPartyDetailedSummary("period_value")
    .Request()
    .GetAsync();

```