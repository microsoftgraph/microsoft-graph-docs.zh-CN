---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 14c710b5f25e27c47c2a824f5b81ff1af607228f
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62114442"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

Get-MgPolicyAppManagementPolicyApplyTo -AppManagementPolicyId $appManagementPolicyId

```