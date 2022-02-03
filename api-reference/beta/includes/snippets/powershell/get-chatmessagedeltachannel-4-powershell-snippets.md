---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3c01815a2e9b7eae066ca98236c5cd52f398bf7a
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62339192"
---
```powershell

Import-Module Microsoft.Graph.Teams

Get-MgTeamChannelMessageDelta -TeamId $teamId -ChannelId $channelId -Deltatoken "aQdvS1VwGCSRxVmZJqykmDik_JIC44iCZpv-GLiA2VnFuE5yG-kCEBROb2iaPT_y_eMWVQtBO_ejzzyIxl00ji-tQ3HzAbW4liZAVG88lO3nG_6-MBFoHY1n8y21YUzjocG-Cn1tCNeeLPLTzIe5Dw.EP9gLiCoF2CE_e6l_m1bTk2aokD9KcgfgfcLGqd1r_4" 

```