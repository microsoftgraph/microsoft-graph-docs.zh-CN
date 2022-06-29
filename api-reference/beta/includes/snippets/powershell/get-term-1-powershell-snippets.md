---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d696994654c8dc66a6cfdafa914f02e71859f5e5
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66441790"
---
```powershell

Import-Module Microsoft.Graph.Sites

Get-MgSiteTermStoreGroupSetTerm -SiteId $siteId -GroupId $groupId -SetId $setId -TermId $termId

```