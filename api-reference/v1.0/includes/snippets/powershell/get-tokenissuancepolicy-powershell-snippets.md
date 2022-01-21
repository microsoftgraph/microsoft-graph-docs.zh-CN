---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c0103a905709c0613040e41cda8cec2ef66e1b4f
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62091561"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

Get-MgPolicyTokenIssuancePolicy -TokenIssuancePolicyId $tokenIssuancePolicyId

```