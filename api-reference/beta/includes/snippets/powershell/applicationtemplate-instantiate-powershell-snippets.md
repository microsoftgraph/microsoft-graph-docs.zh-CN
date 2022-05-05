---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a1f86c69067cf974477559bdcfef63d75cbc14da
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65220254"
---
```powershell

Import-Module Microsoft.Graph.Applications

$params = @{
    DisplayName = "testProperties"
}

Invoke-MgInstantiateApplicationTemplate -ApplicationTemplateId $applicationTemplateId -BodyParameter $params

```