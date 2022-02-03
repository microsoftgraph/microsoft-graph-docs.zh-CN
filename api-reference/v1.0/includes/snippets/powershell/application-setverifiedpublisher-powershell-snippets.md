---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: df853f6c3ae0422a2ac9f5a8144bb02edf6d4488
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62344467"
---
```powershell

Import-Module Microsoft.Graph.Applications

$params = @{
    VerifiedPublisherId = "1234567"
}

Set-MgApplicationVerifiedPublisher -ApplicationId $applicationId -BodyParameter $params

```