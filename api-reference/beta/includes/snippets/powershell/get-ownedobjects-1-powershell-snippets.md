---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b18272e689d6f1fefe5f2fe6e044c22884d542af
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62093212"
---
```powershell

Import-Module Microsoft.Graph.Applications

Get-MgServicePrincipalOwnedObject -ServicePrincipalId $servicePrincipalId

```