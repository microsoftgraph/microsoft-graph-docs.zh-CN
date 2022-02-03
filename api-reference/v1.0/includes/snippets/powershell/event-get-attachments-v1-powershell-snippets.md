---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 507566858f7b07a93e4a02e8f5bd87af0d76abeb
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62349673"
---
```powershell

Import-Module Microsoft.Graph.Calendar

# A UPN can also be used as -UserId.
Get-MgUserEventAttachment -UserId $userId -EventId $eventId

```