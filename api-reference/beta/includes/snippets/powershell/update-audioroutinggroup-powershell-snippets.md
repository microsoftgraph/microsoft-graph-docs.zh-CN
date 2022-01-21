---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 44e630a7197df747aaa42676198497c6d51d86e6
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62116834"
---
```powershell

Import-Module Microsoft.Graph.CloudCommunications

$params = @{
    Id = "oneToOne"
    RoutingMode = "oneToOne"
    Sources = @(
        "632899f8-2ea1-4604-8413-27bd2892079f"
    )
    Receivers = @(
        "550fae72-d251-43ec-868c-373732c2704f"
        "72f988bf-86f1-41af-91ab-2d7cd011db47"
    )
}

Update-MgCommunicationCallAudioRoutingGroup -CallId $callId -AudioRoutingGroupId $audioRoutingGroupId -BodyParameter $params

```