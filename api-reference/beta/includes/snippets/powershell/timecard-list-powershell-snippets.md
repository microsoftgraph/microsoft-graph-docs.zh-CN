---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f572a0aaa78b0b0ecc43f2d9c511cf62adb5cb82
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62108026"
---
```powershell

Import-Module Microsoft.Graph.Teams

Get-MgTeamScheduleTimeCard -TeamId $teamId -Top 2 -Filter "state eq 'clockedOut'" 

```