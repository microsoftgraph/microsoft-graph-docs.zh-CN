---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6a250b6827d4a61aaa5194aa7dff306504a302ef
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62352455"
---
```powershell

Import-Module Microsoft.Graph.Files

# A UPN can also be used as -UserId.
Get-MgUserDrive -UserId $userId

```