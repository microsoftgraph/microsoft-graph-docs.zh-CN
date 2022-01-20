---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2472ef78abf5661bd37d87f55e795f9d3ab4916e
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62104386"
---
```powershell

Import-Module Microsoft.Graph.Sites

Remove-MgSiteTermStoreSet -SiteId $siteId -SetId $setId

```