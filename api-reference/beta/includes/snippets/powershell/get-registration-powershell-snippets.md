---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e4d4e4175a4dc6fd5762e32d62c6589d8740d7c6
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62351565"
---
```powershell

Import-Module Microsoft.Graph.CloudCommunications

# A UPN can also be used as -UserId.
Get-MgUserOnlineMeetingRegistration -UserId $userId -OnlineMeetingId $onlineMeetingId -ExpandProperty "microsoft.graph.meetingRegistration/customQuestions" 

```