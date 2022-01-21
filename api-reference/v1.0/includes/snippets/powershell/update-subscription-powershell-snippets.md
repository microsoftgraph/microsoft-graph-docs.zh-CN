---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5279feb33d13224760edb4eda53856893b64c732
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62128378"
---
```powershell

Import-Module Microsoft.Graph.ChangeNotifications

$params = @{
    ExpirationDateTime = [System.DateTime]::Parse("2016-11-22T18:23:45.9356913Z")
}

Update-MgSubscription -SubscriptionId $subscriptionId -BodyParameter $params

```