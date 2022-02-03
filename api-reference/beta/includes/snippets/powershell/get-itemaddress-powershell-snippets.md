---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3bef29baed7a6d52b1b04859e97c19d8fcb90eaf
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62349478"
---
```powershell

Import-Module Microsoft.Graph.People

# A UPN can also be used as -UserId.
Get-MgUserProfileAddress -UserId $userId -ItemAddressId $itemAddressId

```