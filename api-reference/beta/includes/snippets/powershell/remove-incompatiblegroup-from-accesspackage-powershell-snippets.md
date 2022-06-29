---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a84b10fabf6cfe37dea6be821789001e6cab126b
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66436221"
---
```powershell

Import-Module Microsoft.Graph.Identity.Governance

Remove-MgEntitlementManagementAccessPackageIncompatibleGroupByRef -AccessPackageId $accessPackageId -GroupId $groupId

```