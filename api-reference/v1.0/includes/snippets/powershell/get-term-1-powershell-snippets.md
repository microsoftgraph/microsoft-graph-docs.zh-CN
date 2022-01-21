---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d696994654c8dc66a6cfdafa914f02e71859f5e5
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62087612"
---
```powershell

Import-Module Microsoft.Graph.Sites

Get-MgSiteTermStoreGroupSetTerm -SiteId $siteId -GroupId $groupId -SetId $setId -TermId $termId

```