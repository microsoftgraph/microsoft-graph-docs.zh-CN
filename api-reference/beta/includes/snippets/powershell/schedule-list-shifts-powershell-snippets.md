---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6a3785ae2bde3a37f9cfcaaa79f461941b60f2ec
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62125536"
---
```powershell

Import-Module Microsoft.Graph.Teams

Get-MgTeamScheduleShift -TeamId $teamId -Filter "sharedShift/startDateTime ge 2019-03-11T00:00:00.000Z and sharedShift/endDateTime le 2019-03-18T00:00:00.000Z and draftShift/startDateTime ge 2019-03-11T00:00:00.000Z and draftShift/endDateTime le 2019-03-18T00:00:00.000Z" 

```