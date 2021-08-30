---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6057f1f0da6da14d4dd55742aee33f31330387ef1a4f35914a5a0ef277936319
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278996"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Chats["{chat-id}"].InstalledApps["{teamsAppInstallation-id}"]
    .Upgrade()
    .Request()
    .PostAsync();

```