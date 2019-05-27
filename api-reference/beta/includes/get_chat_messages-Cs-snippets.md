---
description: 自动生成的文件。 不修改
ms.openlocfilehash: afc0f6c62f9c639c5fad8cbc2986e5f57c59aac6
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34472768"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var messages = await graphClient.Chats["{id}"].Messages
    .Request()
    .GetAsync();

```