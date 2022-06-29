---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c2060d0d4ce9a2fd43b7669b0ba1cc693a696579
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66447178"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

Get-MgPolicyRoleManagementPolicyAssignment -Filter "scopeId eq '/' and scopeType eq 'Directory'" 

```