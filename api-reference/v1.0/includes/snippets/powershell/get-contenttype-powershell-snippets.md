---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dbd114da401ec6f9f1eea7741744b084e5152d7e
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62101354"
---
```powershell

Import-Module Microsoft.Graph.Sites

Get-MgSiteContentType -SiteId $siteId -ContentTypeId $contentTypeId

```