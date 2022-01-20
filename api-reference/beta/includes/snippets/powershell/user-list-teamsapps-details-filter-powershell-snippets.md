---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 33cd97095e827622bb45cbbff28070a688c73e08
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62122563"
---
```powershell

Import-Module Microsoft.Graph.Teams

Get-MgUserTeamworkInstalledApp -UserId $userId -ExpandProperty "teamsApp,teamsAppDefinition" -Filter "teamsApp/externalId eq 'cf1ba4c7-f94e-4d80-ba90-5594b641a8ee'" 

```