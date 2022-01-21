---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f6833b3868dd3599df004d1ab6769c289a5bd281
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62105582"
---
```powershell

Import-Module Microsoft.Graph.Applications

Get-MgOnPremisePublishingProfilePublishedResource -OnPremisesPublishingProfileId $onPremisesPublishingProfileId -ExpandProperty "agentGroups" 

```