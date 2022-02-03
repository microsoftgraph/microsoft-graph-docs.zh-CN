---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6b4f499168e22fd91c7b8d11c578425f51dd992b
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62349604"
---
```powershell

Import-Module Microsoft.Graph.Mail

# A UPN can also be used as -UserId.
Get-MgUserMailFolder -UserId $userId

```