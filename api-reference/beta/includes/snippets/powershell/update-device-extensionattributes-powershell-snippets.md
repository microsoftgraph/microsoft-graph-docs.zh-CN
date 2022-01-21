---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e684e3baa4d297895d24ce8d43989762978f7726
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62096861"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

$params = @{
    ExtensionAttributes = @{
        ExtensionAttribute1 = "BYOD-Device"
    }
}

Update-MgDevice -DeviceId $deviceId -BodyParameter $params

```