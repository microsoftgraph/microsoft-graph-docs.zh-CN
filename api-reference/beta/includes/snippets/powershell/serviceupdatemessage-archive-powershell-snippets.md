---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bee271b52b21ad51a8be05fc7cd0957c2e16db39
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63397860"
---
```powershell

Import-Module Microsoft.Graph.Devices.ServiceAnnouncement

$params = @{
    MessageIds = @(
        "MC172851"
        "MC167983"
    )
}

Invoke-MgArchiveServiceAnnouncementMessage -BodyParameter $params

```