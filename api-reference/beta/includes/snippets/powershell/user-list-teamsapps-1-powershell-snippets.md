---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5ec224828f1e31cab51b79906d1ed1589fb60e96
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62095678"
---
```powershell

Import-Module Microsoft.Graph.Teams

Get-MgUserTeamworkInstalledApp -UserId $userId -UserScopeTeamsAppInstallationId $userScopeTeamsAppInstallationId

```