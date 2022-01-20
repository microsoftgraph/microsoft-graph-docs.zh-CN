---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8bc6667871543d3dc5aebf82315c7bf6a231144d
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62121714"
---
```powershell

Import-Module Microsoft.Graph.Sites

Remove-MgSiteTermStoreSetTerm -SiteId $siteId -SetId $setId -TermId $termId

```