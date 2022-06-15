---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d83550357cb6f1f737767b092c24d98382953501
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66095787"
---
```powershell

Import-Module Microsoft.Graph.Users

Get-MgUser -Property "displayName,id" -Filter "identities/any(c:c/issuerAssignedId eq 'j.smith@yahoo.com' and c/issuer eq 'My B2C tenant')" 

```