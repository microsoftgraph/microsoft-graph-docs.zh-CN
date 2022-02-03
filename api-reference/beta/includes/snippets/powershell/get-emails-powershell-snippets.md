---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eae4711904eaba21c321cb3f09e8d2fcda6bb26c
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62349918"
---
```powershell

Import-Module Microsoft.Graph.People

# A UPN can also be used as -UserId.
Get-MgUserProfileEmail -UserId $userId

```