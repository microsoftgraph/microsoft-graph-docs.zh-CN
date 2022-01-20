---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d970bc9795870f614e2be4a3f66400c3ced62cc4
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62125192"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

Get-MgUserAuthenticationSoftwareOathMethod -UserId $userId -SoftwareOathAuthenticationMethodId $softwareOathAuthenticationMethodId

```