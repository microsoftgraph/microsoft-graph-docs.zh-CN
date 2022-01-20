---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: af0cc3b8ddd8a941aca108d0a948b837a31ae3a6
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62102026"
---
```powershell

Import-Module Microsoft.Graph.Teams

Get-MgUserTeamworkInstalledAppChat -UserId $userId -UserScopeTeamsAppInstallationId $userScopeTeamsAppInstallationId

```