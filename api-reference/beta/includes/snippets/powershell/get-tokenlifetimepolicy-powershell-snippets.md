---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f1d84f405ff050eb54ef6e038fefc8fe4653c0dc
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62135006"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

Get-MgPolicyTokenLifetimePolicy -TokenLifetimePolicyId $tokenLifetimePolicyId

```