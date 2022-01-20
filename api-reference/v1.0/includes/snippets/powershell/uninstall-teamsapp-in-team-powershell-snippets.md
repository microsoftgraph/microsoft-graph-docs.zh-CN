---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 43d23f006c7e8d00b429d60b260d24616c4ab97e
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62087878"
---
```powershell

Import-Module Microsoft.Graph.Teams

Remove-MgTeamInstalledApp -TeamId $teamId -TeamsAppInstallationId $teamsAppInstallationId

```