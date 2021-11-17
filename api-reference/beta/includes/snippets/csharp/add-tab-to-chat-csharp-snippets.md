---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4dab9ccfddb01714160f36b88030873713ce409d64524f99932aa4bc14c628b6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218529"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var teamsTab = new TeamsTab
{
    DisplayName = "My Contoso Tab",
    Configuration = new TeamsTabConfiguration
    {
        EntityId = "2DCA2E6C7A10415CAF6B8AB6661B3154",
        ContentUrl = "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/tabView",
        WebsiteUrl = "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154",
        RemoveUrl = "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/uninstallTab"
    },
    AdditionalData = new Dictionary<string, object>()
    {
        {"teamsApp@odata.bind", "https://graph.microsoft.com/beta/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8"}
    }
};

await graphClient.Chats["{chat-id}"].Tabs
    .Request()
    .AddAsync(teamsTab);

```