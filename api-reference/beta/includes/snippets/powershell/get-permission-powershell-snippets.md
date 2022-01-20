---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ca14bcdbc671856cb303726a8337484d440bf3f2
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62126992"
---
```powershell

Import-Module Microsoft.Graph.Sites

Get-MgSitePermission -SiteId $siteId -PermissionId $permissionId

```