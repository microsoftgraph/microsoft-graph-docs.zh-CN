---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3f692e1a8dc7f4e9c0e80924851a36b31dac3d3a
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62128434"
---
```powershell

Import-Module Microsoft.Graph.Sites

Remove-MgSitePermission -SiteId $siteId -PermissionId $permissionId

```