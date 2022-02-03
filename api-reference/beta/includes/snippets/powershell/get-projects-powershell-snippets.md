---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e9d3dd310264c5064ddc0bd2d5cca612457dc5de
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62352169"
---
```powershell

Import-Module Microsoft.Graph.People

# A UPN can also be used as -UserId.
Get-MgUserProfileProject -UserId $userId

```