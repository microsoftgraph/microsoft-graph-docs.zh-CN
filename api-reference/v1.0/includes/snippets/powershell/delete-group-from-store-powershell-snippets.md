---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 254ba41ffaf74c4b85cce9b27d577c2853e0c22a
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62110597"
---
```powershell

Import-Module Microsoft.Graph.Sites

Remove-MgSiteTermStoreGroup -SiteId $siteId -GroupId $groupId

```