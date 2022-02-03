---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a9b4c9374e200b5fc87393c4ea5358c726c02fcc
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62344243"
---
```powershell

Import-Module Microsoft.Graph.Sites

Publish-MgSiteContentType -SiteId $siteId -ContentTypeId $contentTypeId

```