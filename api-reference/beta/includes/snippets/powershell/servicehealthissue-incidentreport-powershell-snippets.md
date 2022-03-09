---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 22527b011cf664448f40746ab9c56e21f15474f4
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63396719"
---
```powershell

Import-Module Microsoft.Graph.Devices.ServiceAnnouncement

Invoke-MgReportServiceAnnouncementIssueIncident -ServiceHealthIssueId $serviceHealthIssueId

```