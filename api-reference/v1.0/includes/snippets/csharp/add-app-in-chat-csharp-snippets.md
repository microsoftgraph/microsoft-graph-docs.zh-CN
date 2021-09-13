---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aed290a892e17f6b5114cc69f556e90a3bb266692f802249b632c72a7b673efc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104335"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var teamsAppInstallation = new TeamsAppInstallation
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"teamsApp@odata.bind", "https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/12345678-9abc-def0-123456789a"}
    }
};

await graphClient.Chats["{chat-id}"].InstalledApps
    .Request()
    .AddAsync(teamsAppInstallation);

```