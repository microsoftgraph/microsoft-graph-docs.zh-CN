---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ad05275e65912947bb0d88c6706681a121f7e534
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62099758"
---
```powershell

Import-Module Microsoft.Graph.Identity.Governance

Get-MgEntitlementManagementAccessPackageResourceEnvironment -Filter "originSystem eq 'SharePointOnline'" 

```