---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e54f9386a3ba566a38c8979c59d711dd89a7228c
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62102698"
---
```powershell

Import-Module Microsoft.Graph.Applications

Get-MgOnPremisePublishingProfileAgent -OnPremisesPublishingProfileId $onPremisesPublishingProfileId -OnPremisesAgentId $onPremisesAgentId -ExpandProperty "agentGroups" 

```