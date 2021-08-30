---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e40c4e086c2e1b30e436079869bd95a91b38b908ae903e18b399f852b1e59975
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158557"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var teamsAppInstallation = new TeamsAppInstallation
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"teamsApp@odata.bind", "https://graph.microsoft.com/beta/appCatalogs/teamsApps/12345678-9abc-def0-123456789a"}
    }
};

await graphClient.Chats["{chat-id}"].InstalledApps
    .Request()
    .AddAsync(teamsAppInstallation);

```