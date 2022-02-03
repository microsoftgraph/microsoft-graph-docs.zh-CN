---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b4db87791db03e0aa908e0cf267c91b58284d85c
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62342385"
---
```powershell

Import-Module Microsoft.Graph.Sites

Restore-MgSiteListItemVersion -SiteId $siteId -ListId $listId -ListItemId $listItemId -ListItemVersionId $listItemVersionId

```