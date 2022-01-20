---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a2726a50ce6213188b3d180bae3326b231515fd1
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62117773"
---
```powershell

Import-Module Microsoft.Graph.Sites

Get-MgSiteContentTypeColumn -SiteId $siteId -ContentTypeId $contentTypeId

```