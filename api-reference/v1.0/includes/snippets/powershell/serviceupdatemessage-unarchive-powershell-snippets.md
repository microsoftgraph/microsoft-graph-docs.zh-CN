---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0c6cedd1d229454738dd493cac2e507629ea966e
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63396404"
---
```powershell

Import-Module Microsoft.Graph.Devices.ServiceAnnouncement

$params = @{
    MessageIds = @(
        "MC172851"
        "MC167983"
    )
}

Invoke-MgUnarchiveServiceAnnouncementMessage -BodyParameter $params

```