---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9a49ee2ec5b6cb37b8910cdb03448155aefca1b2
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62352366"
---
```powershell

Import-Module Microsoft.Graph.CloudCommunications

# A UPN can also be used as -UserId.
Get-MgUserOnlineMeetingRegistration -UserId $userId -OnlineMeetingId $onlineMeetingId

```