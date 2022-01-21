---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d67cb577fcbaa609686824fbcbcbe89bc7a3a75e
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62124895"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

Get-MgIdentityConditionalAccessNamedLocation -Filter "createdDateTime ge 2019-09-01T00:00:00Z" 

```