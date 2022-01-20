---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3fe501940387b341b55a0071e3d360c82861fb8e
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62091658"
---
```powershell

Import-Module Microsoft.Graph.ChangeNotifications

$params = @{
    ChangeType = "created"
    NotificationUrl = "https://webhook.azurewebsites.net/api/send/myNotifyClient"
    Resource = "me/mailFolders('Inbox')/messages"
    ExpirationDateTime = [System.DateTime]::Parse("2016-11-20T18:23:45.9356913Z")
    ClientState = "secretClientValue"
    LatestSupportedTlsVersion = "v1_2"
}

New-MgSubscription -BodyParameter $params

```