---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e94b97017d40d1f5273049483c3ec80717cd2f38
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62345710"
---
```powershell

Import-Module Microsoft.Graph.CloudCommunications

$params = @{
    Role = "viewer"
}

Rename-MgCommunicationCallScreenSharingRole -CallId $callId -BodyParameter $params

```