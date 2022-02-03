---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1ccdc752da11988f2a9aae5ed9941db94f80a42e
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62350264"
---
```powershell

Import-Module Microsoft.Graph.People

# A UPN can also be used as -UserId.
Get-MgUserProfileEducationalActivity -UserId $userId

```