---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6bec10e5dc7f9f6f26c871d4a06d4a28678e16e1
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62087983"
---
```powershell

Import-Module Microsoft.Graph.Applications

Get-MgServicePrincipalOwner -ServicePrincipalId $servicePrincipalId

```