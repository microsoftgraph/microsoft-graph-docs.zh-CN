---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 432f553fdfdc839c92c7d4a9de9ed7e624fca0d3
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62091330"
---
```powershell

Import-Module Microsoft.Graph.Teams

Remove-MgUserTeamworkInstalledApp -UserId $userId -UserScopeTeamsAppInstallationId $userScopeTeamsAppInstallationId

```