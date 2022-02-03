---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 838bacccb009dcb8e80563b1683981104b290235
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62352453"
---
```powershell

Import-Module Microsoft.Graph.Users

# A UPN can also be used as -UserId.
Get-MgUserOwnedObject -UserId $userId

```