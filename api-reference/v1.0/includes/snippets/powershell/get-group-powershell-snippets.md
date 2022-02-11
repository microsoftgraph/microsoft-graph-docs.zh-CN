---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e481c140a292e3217dfb8ba767b9a81c59cf439a
ms.sourcegitcommit: 4e16f26b6b685a6a3dae855a04979c84105609b9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/10/2022
ms.locfileid: "62530456"
---
```powershell

Import-Module Microsoft.Graph.Sites

Get-MgSiteTermStoreGroup -SiteId $siteId -GroupId $groupId -Property "*,parentSiteId" 

```