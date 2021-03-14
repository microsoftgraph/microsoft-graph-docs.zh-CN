---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 86e5b34d788c2049d8dfae868b6acc405e3004fe
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50795116"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var conversation = await graphClient.Groups["{group-id}"].Conversations["{conversation-id}"]
    .Request()
    .GetAsync();

```