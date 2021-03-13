---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e2c856adef8786b2c09dc47ddb1ae0f02b47ae3e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50791407"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var channel = await graphClient.Teams["{team-id}"].Channels["{channel-id}"]
    .Request()
    .GetAsync();

```