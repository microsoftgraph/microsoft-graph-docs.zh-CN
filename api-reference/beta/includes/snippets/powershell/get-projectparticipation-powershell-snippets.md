---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 63d00599b5799cf351671cc6638e8178c4883b23
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62112095"
---
```powershell

Import-Module Microsoft.Graph.People

Get-MgUserProfileProject -UserId $userId -ProjectParticipationId $projectParticipationId

```