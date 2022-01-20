---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2ee6fdb94159c93388166a3ec3b9b1cbd30071c1
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62126516"
---
```powershell

Import-Module Microsoft.Graph.WindowsUpdates

Remove-MgWindowsUpdatesDeployment -DeploymentId $deploymentId

```