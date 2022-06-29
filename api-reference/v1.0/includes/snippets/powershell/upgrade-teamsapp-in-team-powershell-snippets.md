---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c51458d856b2f9c7b70e9c1fbe6c99c85c3d0222
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66441090"
---
```powershell

Import-Module Microsoft.Graph.Teams

Update-MgTeamInstalledApp -TeamId $teamId -TeamsAppInstallationId $teamsAppInstallationId

```