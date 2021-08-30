---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d25de9a558d7cfbcfff69c5c3ce906f95a76b2824d1694c5765561369913aecd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220942"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Chats["{chat-id}"].InstalledApps["{teamsAppInstallation-id}"]
    .Request()
    .DeleteAsync();

```