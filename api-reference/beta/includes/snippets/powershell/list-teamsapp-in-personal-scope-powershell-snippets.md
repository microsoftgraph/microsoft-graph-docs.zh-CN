---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 15338df3a55588dd73a4f64cbf488531ce001047
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62110080"
---
```powershell

Import-Module Microsoft.Graph.Teams

Get-MgAppCatalogTeamApp -ExpandProperty "appDefinitions(`$select=id,displayName,allowedInstallationScopes)" -Filter "appDefinitions/any(a:a/allowedInstallationScopes has 'personal')" 

```