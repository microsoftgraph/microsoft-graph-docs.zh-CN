---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c45fcc38ddb51addc417be94c54aac2c5a8ab451
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62347269"
---
```powershell

Import-Module Microsoft.Graph.Sites

Unpublish-MgSiteContentType -SiteId $siteId -ContentTypeId $contentTypeId

```