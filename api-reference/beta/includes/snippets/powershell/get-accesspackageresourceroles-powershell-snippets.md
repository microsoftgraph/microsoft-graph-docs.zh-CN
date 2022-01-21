---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ec5a03363101a9540a3ece157a517ee2b168de94
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62097436"
---
```powershell

Import-Module Microsoft.Graph.Identity.Governance

Get-MgEntitlementManagementAccessPackageCatalogAccessPackageResourceRole -AccessPackageCatalogId $accessPackageCatalogId -Filter "(originSystem eq 'AadGroup' and accessPackageResource/id eq 'a35bef72-a8aa-4ca3-af30-f6b2ece7208f')" -ExpandProperty "accessPackageResource" 

```