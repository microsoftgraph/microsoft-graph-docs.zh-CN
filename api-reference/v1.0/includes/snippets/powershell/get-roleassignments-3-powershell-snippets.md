---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dd07bc65c4c57cbb320397ca3463d5faa1ba4b9e
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65207433"
---
```powershell

Import-Module Microsoft.Graph.DeviceManagement.Enrolment

Get-MgRoleManagementEntitlementManagementRoleAssignment -Filter "appScopeId eq '/AccessPackageCatalog/4cee616b-fdf9-4890-9d10-955e0ccb12bc'" -ExpandProperty "principal" 

```