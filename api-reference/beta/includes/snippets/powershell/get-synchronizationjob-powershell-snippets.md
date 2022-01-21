---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 150f278488a4ea68d7c73cf766bcbf4510bca171
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62130764"
---
```powershell

Import-Module Microsoft.Graph.Applications

Get-MgServicePrincipalSynchronizationJob -ServicePrincipalId $servicePrincipalId -SynchronizationJobId $synchronizationJobId

```