---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 57aaa68bda16e2dbad98aeabb1a827f68b4ce2e5
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62114702"
---
```powershell

Import-Module Microsoft.Graph.CloudCommunications

Get-MgUserOnlineMeetingAttendeeReport -UserId $userId -OnlineMeetingId $onlineMeetingId

```