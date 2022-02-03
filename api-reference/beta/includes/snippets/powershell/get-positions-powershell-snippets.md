---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 51e8083a4a5f8f34b1329bd66d83bc9af53eb791
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62350098"
---
```powershell

Import-Module Microsoft.Graph.People

# A UPN can also be used as -UserId.
Get-MgUserProfilePosition -UserId $userId

```