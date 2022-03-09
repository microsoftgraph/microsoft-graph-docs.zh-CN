---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e66450f020c4120d8f46dfca82a1df6bf159ca36
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63393611"
---
```powershell

Import-Module Microsoft.Graph.Devices.ServiceAnnouncement

Get-MgServiceAnnouncementHealthOverview -ExpandProperty "issues" 

```