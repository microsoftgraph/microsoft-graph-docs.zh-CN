---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9d0e27bb9da96f5961d486defe5fd72ee9554773
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62088053"
---
```powershell

Import-Module Microsoft.Graph.Teams

Get-MgTeamScheduleTimeOff -TeamId $teamId -Filter "sharedTimeOff/startDateTime ge 2019-03-11T00:00:00.000Z and sharedTimeOff/endDateTime le 2019-03-18T00:00:00.000Z and draftTimeOff/startDateTime ge 2019-03-11T00:00:00.000Z and draftTimeOff/endDateTime le 2019-03-18T00:00:00.000Z" 

```