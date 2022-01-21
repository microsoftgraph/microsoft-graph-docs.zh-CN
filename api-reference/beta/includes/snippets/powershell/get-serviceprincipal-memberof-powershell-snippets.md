---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3314a4b5939a336fde26cc5cbc07ae19fc8c7f91
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62129441"
---
```powershell

Import-Module Microsoft.Graph.Applications

Get-MgServicePrincipalMemberOf -ServicePrincipalId $servicePrincipalId

```