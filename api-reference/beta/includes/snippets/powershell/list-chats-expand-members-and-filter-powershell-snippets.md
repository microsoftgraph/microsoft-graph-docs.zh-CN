---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 833dbdd46860681f4e8812078db4aea3ddb9eaf4
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62094446"
---
```powershell

Import-Module Microsoft.Graph.Teams

Get-MgUserChat -UserId $userId -ExpandProperty "members" -Filter "members/any(o: o/displayname eq 'Peter Parker')" 

```