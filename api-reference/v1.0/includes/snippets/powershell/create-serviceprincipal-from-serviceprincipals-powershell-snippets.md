---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e98e88350c4cc3592a8ba9d6b112ec33a1e13abf
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62128532"
---
```powershell

Import-Module Microsoft.Graph.Applications

$params = @{
    AppId = "65415bb1-9267-4313-bbf5-ae259732ee12"
}

New-MgServicePrincipal -BodyParameter $params

```