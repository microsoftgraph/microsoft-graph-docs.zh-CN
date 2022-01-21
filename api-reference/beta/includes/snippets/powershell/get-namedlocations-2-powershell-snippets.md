---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 58258c172fc66e51e81fe47cea77324a53b88bb5
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62109248"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

Get-MgIdentityConditionalAccessNamedLocation -Filter "isof('microsoft.graph.ipNamedLocation')" 

```