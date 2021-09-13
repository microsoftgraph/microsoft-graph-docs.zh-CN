---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: be54f98e68a42b0579abd6519a633906135466080371e65733e22311326dfce3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274086"
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
        {"teamsApp@odata.bind", "https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8"}
    }
};

await graphClient.Chats["{chat-id}"].Tabs
    .Request()
    .AddAsync(teamsTab);

```