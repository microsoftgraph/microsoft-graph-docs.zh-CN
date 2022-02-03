---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8f32c59375a22628d4299e66fdfef3d0ebfa1139
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62349864"
---
```powershell

Import-Module Microsoft.Graph.People

# A UPN can also be used as -UserId.
Remove-MgUserProfileWebsite -UserId $userId -PersonWebsiteId $personWebsiteId

```