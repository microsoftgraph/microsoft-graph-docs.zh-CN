---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8666a9572ef936d408c4b315a74cd08d8f9075cb
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62349081"
---
```powershell

Import-Module Microsoft.Graph.Applications

Invoke-MgFilterServicePrincipalSynchronizationJobSchemaOperator -ServicePrincipalId $servicePrincipalId -SynchronizationJobId $synchronizationJobId

```