---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 01cc9036cc15912315eb0787e28de86615041ef1
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62349977"
---
```powershell

Import-Module Microsoft.Graph.People

# A UPN can also be used as -UserId.
Get-MgUserProfileAward -UserId $userId

```