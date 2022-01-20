---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2095b8b6862522960542dc53af5339186247d1a4
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62126640"
---
```powershell

Import-Module Microsoft.Graph.Users

Get-MgUser -Filter "endswith(mail,'a@contoso.com')" -Sort "userPrincipalName" -CountVariable CountVar -ConsistencyLevel eventual 


```