---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a8385512388c5e5878fa99e6d078d7271efd2454
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62090945"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

Remove-MgPolicyActivityBasedTimeoutPolicy -ActivityBasedTimeoutPolicyId $activityBasedTimeoutPolicyId

```