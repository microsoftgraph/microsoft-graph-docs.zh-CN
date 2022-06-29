---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4e1de1a3d7b9aaddbbaf4f880537f30f33e773b6
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66447198"
---
```powershell

Import-Module Microsoft.Graph.Sites

Get-MgSiteListContentTypeCompatibleHubContentType -SiteId $siteId -ListId $listId

```