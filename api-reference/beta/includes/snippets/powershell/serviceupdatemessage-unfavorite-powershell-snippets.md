---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7cf6332c48c4b6499bee58073fb4276e90523bdc
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63397573"
---
```powershell

Import-Module Microsoft.Graph.Devices.ServiceAnnouncement

$params = @{
    MessageIds = @(
        "MC172851"
        "MC167983"
    )
}

Invoke-MgUnfavoriteServiceAnnouncementMessage -BodyParameter $params

```