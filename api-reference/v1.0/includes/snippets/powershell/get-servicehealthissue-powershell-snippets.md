---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a3e2a0f594aea8b2348886bdee9d8512ec4f4d9f
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63394577"
---
```powershell

Import-Module Microsoft.Graph.Devices.ServiceAnnouncement

Get-MgServiceAnnouncementIssue -ServiceHealthIssueId $serviceHealthIssueId

```