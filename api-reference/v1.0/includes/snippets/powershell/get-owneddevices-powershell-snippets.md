---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 733e8e69a2a0878eecd28d11fd51132a39aef32f
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62349310"
---
```powershell

Import-Module Microsoft.Graph.Users

# A UPN can also be used as -UserId.
Get-MgUserOwnedDevice -UserId $userId

```