---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7e328fd8b301ee7a96d1d6c6ef72c23f7d86229b
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62129274"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

Remove-MgPolicyTokenIssuancePolicy -TokenIssuancePolicyId $tokenIssuancePolicyId

```