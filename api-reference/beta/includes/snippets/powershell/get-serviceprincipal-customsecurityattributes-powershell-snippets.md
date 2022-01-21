---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e706eb2c114d22202d0375f8810d29765d97b5dc
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62098925"
---
```powershell

Import-Module Microsoft.Graph.Applications

Get-MgServicePrincipal -ServicePrincipalId $servicePrincipalId -Property "customSecurityAttributes" 

```