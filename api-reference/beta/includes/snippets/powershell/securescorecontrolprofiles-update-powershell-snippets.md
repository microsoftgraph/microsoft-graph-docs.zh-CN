---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 25a956bab1fd79c7759b4b52605b78f24beb76c8
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62089354"
---
```powershell

Import-Module Microsoft.Graph.Security

$params = @{
    ControlStateUpdates = "controlStateUpdates-value"
}

Update-MgSecuritySecureScoreControlProfile -SecureScoreControlProfileId $secureScoreControlProfileId -BodyParameter $params

```