---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 662f6a3cce7d097440eff62b855d54c3e8704dbb
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62097183"
---
```powershell

Import-Module Microsoft.Graph.Teams

Get-MgTeamChannel -TeamId $teamId -Filter "membershipType eq 'private'" 

```