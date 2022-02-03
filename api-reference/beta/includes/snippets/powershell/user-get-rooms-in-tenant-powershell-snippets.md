---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f3bc1947594eb6d080cd2f8120c7cefc73e9c79f
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62339112"
---
```powershell

Import-Module Microsoft.Graph.Users.Functions

# A UPN can also be used as -UserId.
Find-MgUserRoom -UserId $userId

```