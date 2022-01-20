---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d5ff3b295eaa1811890263910154c7d637d4e4a7
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62111814"
---
```powershell

Import-Module Microsoft.Graph.Applications

Get-MgServicePrincipalTransitiveMemberOf -ServicePrincipalId $servicePrincipalId

```