---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 00a72138333e25910fc5f2cad72d816abfb5fe6c
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62112921"
---
```powershell

Import-Module Microsoft.Graph.Applications

Get-MgOnPremisePublishingProfile -OnPremisesPublishingProfileId $onPremisesPublishingProfileId -ExpandProperty "publishedResources,agents,agentGroups" 

```