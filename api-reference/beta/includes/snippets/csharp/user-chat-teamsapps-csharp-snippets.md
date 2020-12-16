---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8d33f7ecc5ece06f3e7419385b7a0897f12c6cd8
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "49690279"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var chat = await graphClient.Users["f32b83bb-4fc8-4db7-b7f5-76cdbbb8aa1c"].Teamwork.InstalledApps["ZjMyYjgzYmItNGZjOC00ZGI3LWI3ZjUtNzZjZGJiYjhhYTFjIyMyMmY3M2JiZS1mNjdhLTRkZWEtYmQ1NC01NGNhYzcxOGNiMmI="].Chat
    .Request()
    .GetAsync();

```