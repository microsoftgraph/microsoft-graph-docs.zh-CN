---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 18e1efbf61e70901dfa899d9a7aba0a4ef06f3b3
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62348746"
---
```powershell

Import-Module Microsoft.Graph.Applications

Start-MgServicePrincipalSynchronizationJob -ServicePrincipalId $servicePrincipalId -SynchronizationJobId $synchronizationJobId

```