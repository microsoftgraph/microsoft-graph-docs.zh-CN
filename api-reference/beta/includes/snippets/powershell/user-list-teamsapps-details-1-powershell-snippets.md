---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 543b270f2a28d222b3e20819845ce6ba210db3d2
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62095679"
---
```powershell

Import-Module Microsoft.Graph.Teams

Get-MgUserTeamworkInstalledApp -UserId $userId -UserScopeTeamsAppInstallationId $userScopeTeamsAppInstallationId -ExpandProperty "teamsAppDefinition" 

```