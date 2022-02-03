---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a1eaa077f2c8fcfc46f798a0e97b3958a5d2195e
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62347086"
---
```powershell

Import-Module Microsoft.Graph.Applications

Suspend-MgServicePrincipalSynchronizationJob -ServicePrincipalId $servicePrincipalId -SynchronizationJobId $synchronizationJobId

```