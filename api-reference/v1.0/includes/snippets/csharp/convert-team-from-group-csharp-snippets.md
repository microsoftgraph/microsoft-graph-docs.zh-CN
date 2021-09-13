---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 913af59ec2015fabfee402127c87813187db8f196c6f5abc2c6e10290164aa66
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903225"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var team = new Team
{
    Channels = new TeamChannelsCollectionPage()
    {
        new Channel
        {
            DisplayName = "Class Announcements 📢",
            IsFavoriteByDefault = true
        },
        new Channel
        {
            DisplayName = "Homework 🏋️",
            IsFavoriteByDefault = true
        }
    },
    MemberSettings = new TeamMemberSettings
    {
        AllowCreateUpdateChannels = false,
        AllowDeleteChannels = false,
        AllowAddRemoveApps = false,
        AllowCreateUpdateRemoveTabs = false,
        AllowCreateUpdateRemoveConnectors = false
    },
    InstalledApps = new TeamInstalledAppsCollectionPage()
    {
        new TeamsAppInstallation
        {
            AdditionalData = new Dictionary<string, object>()
            {
                {"teamsApp@odata.bind", "https://graph.microsoft.com/v1.0/appCatalogs/teamsApps('com.microsoft.teamspace.tab.vsts')"}
            }
        },
        new TeamsAppInstallation
        {
            AdditionalData = new Dictionary<string, object>()
            {
                {"teamsApp@odata.bind", "https://graph.microsoft.com/v1.0/appCatalogs/teamsApps('1542629c-01b3-4a6d-8f76-1938b779e48d')"}
            }
        }
    },
    AdditionalData = new Dictionary<string, object>()
    {
        {"template@odata.bind", "https://graph.microsoft.com/v1.0/teamsTemplates('standard')"},
        {"group@odata.bind", "https://graph.microsoft.com/v1.0/groups('dbd8de4f-5d47-48da-87f1-594bed003375')"}
    }
};

await graphClient.Teams
    .Request()
    .AddAsync(team);

```