---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 97ee77ebe022f5f8c0f35be6bef959d94bf8d000aa97cc7fe2b4fc799eb23080
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279528"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Teams["{team-id}"].Channels["{channel-id}"]
    .CompleteMigration()
    .Request()
    .PostAsync();

```