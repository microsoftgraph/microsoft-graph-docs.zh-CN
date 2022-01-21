---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fb0176e1d7494451ad70dd746695fa84bc272034
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62107613"
---
```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
    DisplayName = "My Contoso Tab"
    "TeamsApp@odata.bind" = "https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8"
    Configuration = @{
        EntityId = "2DCA2E6C7A10415CAF6B8AB6661B3154"
        ContentUrl = "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/tabView"
        WebsiteUrl = "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154"
        RemoveUrl = "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/uninstallTab"
    }
}

New-MgChatTab -ChatId $chatId -BodyParameter $params

```