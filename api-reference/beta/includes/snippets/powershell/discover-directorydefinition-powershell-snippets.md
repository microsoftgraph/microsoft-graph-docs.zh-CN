---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: da8386c12a344c87fed6f67256c5b8b2472ac54a
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62345673"
---
```powershell

Import-Module Microsoft.Graph.Applications

Find-MgServicePrincipalSynchronizationJobSchemaDirectory -ServicePrincipalId $servicePrincipalId -SynchronizationJobId $synchronizationJobId -DirectoryDefinitionId $directoryDefinitionId

```