---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1c918122af4e7aa7af7371ca2efa64b299909320
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62113581"
---
```powershell

Import-Module Microsoft.Graph.CloudCommunications

Remove-MgUserOnlineMeetingRegistration -UserId $userId -OnlineMeetingId $onlineMeetingId

```