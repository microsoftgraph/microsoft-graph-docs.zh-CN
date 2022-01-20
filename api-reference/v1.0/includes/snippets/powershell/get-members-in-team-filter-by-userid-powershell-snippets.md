---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 86ac039690cd9a820c1288286f45906a97cc5545
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62131910"
---
```powershell

Import-Module Microsoft.Graph.Teams

Get-MgTeamMember -TeamId $teamId -Filter "(microsoft.graph.aadUserConversationMember/userId eq '73761f06-2ac9-469c-9f10-279a8cc267f9')" 

```