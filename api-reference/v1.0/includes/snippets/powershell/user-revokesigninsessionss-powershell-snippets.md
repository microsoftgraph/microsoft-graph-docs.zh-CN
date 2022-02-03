---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c7b4063eb33756c34a5facdc481b2ac83c255ccb
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62343568"
---
```powershell

Import-Module Microsoft.Graph.Users.Actions

# A UPN can also be used as -UserId.
Revoke-MgUserSign -UserId $userId

```