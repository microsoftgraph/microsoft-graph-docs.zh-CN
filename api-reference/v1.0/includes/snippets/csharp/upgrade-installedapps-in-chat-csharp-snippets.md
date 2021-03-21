---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6a8640d4dd9fa2cbf1e5e585ce9f04cc4b5d5265
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960010"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Chats["{chat-id}"].InstalledApps["{teamsAppInstallation-id}"]
    .Upgrade()
    .Request()
    .PostAsync();

```