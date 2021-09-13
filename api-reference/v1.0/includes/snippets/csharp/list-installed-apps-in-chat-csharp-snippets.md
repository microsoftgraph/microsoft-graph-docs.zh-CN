---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4bba9e7b7402e0f3df7e53c9319c8e7e35eede04c9db72d275fcd163500de3c0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106827"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var installedApps = await graphClient.Chats["{chat-id}"].InstalledApps
    .Request()
    .GetAsync();

```