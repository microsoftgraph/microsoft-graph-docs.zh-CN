---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 986eed3514664cb38c3ed311001f867d751d2bb5
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66445699"
---
```powershell

Import-Module Microsoft.Graph.Sites

Remove-MgSiteListItemDocumentSetVersion -SiteId $siteId -ListId $listId -ListItemId $listItemId -DocumentSetVersionId $documentSetVersionId

```