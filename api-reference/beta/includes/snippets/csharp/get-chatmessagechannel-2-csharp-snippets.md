---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 88f7638932661c2e78e2ffac5adb99987cde8e93ce4ab571d7537f9e3167aabf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163175"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var chatMessage = await graphClient.Teams["{team-id}"].Channels["{channel-id}"].Messages["{chatMessage-id}"]
    .Request()
    .GetAsync();

```