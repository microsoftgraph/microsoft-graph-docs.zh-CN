---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c32ca2521b14afb22ab7dc99408949ae167f7c80
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66447366"
---
```powershell

Import-Module Microsoft.Graph.Sites

Get-MgSiteListItemDocumentSetVersion -SiteId $siteId -ListId $listId -ListItemId $listItemId

```