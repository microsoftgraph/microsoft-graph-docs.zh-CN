---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 85c298f3a80a8085ba7875427c2c93bd408ff256
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63395900"
---
```powershell

Import-Module Microsoft.Graph.Devices.ServiceAnnouncement

Get-MgServiceAnnouncementMessage -ServiceUpdateMessageId $serviceUpdateMessageId

```