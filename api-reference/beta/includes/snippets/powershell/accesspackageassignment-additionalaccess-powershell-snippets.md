---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 619db03cd890e09d33aae5e62c9655815579b35a
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65203785"
---
```powershell

Import-Module Microsoft.Graph.Identity.Governance

Get-MgEntitlementManagementAccessPackageAssignment -AccessPackageAssignmentId $accessPackageAssignmentId -ExpandProperty "target" 

```