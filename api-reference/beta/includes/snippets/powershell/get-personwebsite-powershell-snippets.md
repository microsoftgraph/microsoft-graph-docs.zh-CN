---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1210e62895e9f0e15aa05595d2a22a980d85ad65
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62350844"
---
```powershell

Import-Module Microsoft.Graph.People

# A UPN can also be used as -UserId.
Get-MgUserProfileWebsite -UserId $userId -PersonWebsiteId $personWebsiteId

```