---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9c31b31d153f73ec16c1dd6f7b3bd1a7ab513639
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62106632"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

Remove-MgIdentityConditionalAccessPolicy -ConditionalAccessPolicyId $conditionalAccessPolicyId

```