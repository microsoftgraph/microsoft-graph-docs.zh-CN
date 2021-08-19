---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8c7acdb81abe246a50c7d8d5fdeeaa7a6e447c30807bab86de7435d4113e3210
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218516"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var hostedContents = await graphClient.Teams["{team-id}"].Channels["{channel-id}"].Messages["{chatMessage-id}"].HostedContents
    .Request()
    .GetAsync();

```