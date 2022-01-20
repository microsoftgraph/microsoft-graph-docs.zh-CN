---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b00e69f4b84ba3e8c028d197b140ff6367224fd2
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62111723"
---
```powershell

Import-Module Microsoft.Graph.Sites

Get-MgSite -Property "siteCollection,webUrl" -Filter "siteCollection/root ne null" 

```