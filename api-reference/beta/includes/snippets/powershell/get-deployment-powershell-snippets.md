---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9f04334dae250ced156a4e57ab3d65d95472c55a
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62088998"
---
```powershell

Import-Module Microsoft.Graph.WindowsUpdates

Get-MgWindowsUpdatesDeployment -DeploymentId $deploymentId

```