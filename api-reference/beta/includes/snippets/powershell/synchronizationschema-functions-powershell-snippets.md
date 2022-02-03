---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 86a1e5216512194e941f85ab1886ac832faa627c
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62349083"
---
```powershell

Import-Module Microsoft.Graph.Applications

Invoke-MgFunctionServicePrincipalSynchronizationJobSchema -ServicePrincipalId $servicePrincipalId -SynchronizationJobId $synchronizationJobId

```