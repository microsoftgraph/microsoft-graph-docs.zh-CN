---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7ed06a678d518f2da2fb9e1c67f223a6878d53f8
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338358"
---
```powershell

Import-Module Microsoft.Graph.Identity.Governance

Remove-MgEntitlementManagementAccessPackageCatalogCustomAccessPackageWorkflowExtension -AccessPackageCatalogId $accessPackageCatalogId -CustomAccessPackageWorkflowExtensionId $customAccessPackageWorkflowExtensionId

```