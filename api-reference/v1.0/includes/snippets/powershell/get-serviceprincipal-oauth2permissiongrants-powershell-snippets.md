---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0ac725d8f4fd3b496ff072617d0c18001865f974
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62121952"
---
```powershell

Import-Module Microsoft.Graph.Applications

Get-MgServicePrincipalOauth2PermissionGrant -ServicePrincipalId $servicePrincipalId

```