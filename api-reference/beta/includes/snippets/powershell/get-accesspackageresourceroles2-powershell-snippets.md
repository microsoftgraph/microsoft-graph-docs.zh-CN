---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e9614d792e74667ec4d552bfcc87ff6d775b013c
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62097434"
---
```powershell

Import-Module Microsoft.Graph.Identity.Governance

Get-MgEntitlementManagementAccessPackageCatalogAccessPackageResourceRole -AccessPackageCatalogId $accessPackageCatalogId -Filter "(originSystem eq 'SharePointOnline' and accessPackageResource/id eq '53c71803-a0a8-4777-aecc-075de8ee3991')" -Property "displayName,originId" 

```