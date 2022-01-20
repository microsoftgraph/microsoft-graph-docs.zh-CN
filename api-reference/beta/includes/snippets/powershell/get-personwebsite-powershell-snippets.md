---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ccace6120facfbac38805ddaa2664d3a5c2d52c1
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62093906"
---
```powershell

Import-Module Microsoft.Graph.People

Get-MgUserProfileWebsite -UserId $userId -PersonWebsiteId $personWebsiteId

```