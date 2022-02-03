---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fe8e264a7daa707103a93c462314280025c4ba45
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62339291"
---
```powershell

Import-Module Microsoft.Graph.Applications

$params = @{
    DisplayName = "My custom name"
}

Invoke-MgInstantiateApplicationTemplate -ApplicationTemplateId $applicationTemplateId -BodyParameter $params

```