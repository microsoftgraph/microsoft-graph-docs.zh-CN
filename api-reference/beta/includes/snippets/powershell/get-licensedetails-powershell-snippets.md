---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a414e9b90b22d202c4b58f3eab7d1c0a931d0871
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62349338"
---
```powershell

Import-Module Microsoft.Graph.Users

# A UPN can also be used as -UserId.
Get-MgUserLicenseDetail -UserId $userId

```