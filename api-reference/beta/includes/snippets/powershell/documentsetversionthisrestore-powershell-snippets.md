---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ccbed2000acce64824cee253378eee101b883ff8
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66445678"
---
```powershell

Import-Module Microsoft.Graph.Sites

Restore-MgSiteListItemDocumentSetVersion -SiteId $siteId -ListId $listId -ListItemId $listItemId -DocumentSetVersionId $documentSetVersionId

```