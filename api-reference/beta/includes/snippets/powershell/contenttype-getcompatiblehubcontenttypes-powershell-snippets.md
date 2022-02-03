---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4e1de1a3d7b9aaddbbaf4f880537f30f33e773b6
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62339839"
---
```powershell

Import-Module Microsoft.Graph.Sites

Get-MgSiteListContentTypeCompatibleHubContentType -SiteId $siteId -ListId $listId

```