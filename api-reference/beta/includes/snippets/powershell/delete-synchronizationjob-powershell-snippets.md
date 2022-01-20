---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a0d4a88a4618ccf8d76c25fc3127094fd0e0211b
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62098721"
---
```powershell

Import-Module Microsoft.Graph.Applications

Remove-MgServicePrincipalSynchronizationJob -ServicePrincipalId $servicePrincipalId -SynchronizationJobId $synchronizationJobId

```