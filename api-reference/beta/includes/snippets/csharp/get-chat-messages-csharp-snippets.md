---
description: 自动生成的文件。 不修改
ms.openlocfilehash: afc0f6c62f9c639c5fad8cbc2986e5f57c59aac6
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35520387"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var messages = await graphClient.Chats["{id}"].Messages
    .Request()
    .GetAsync();

```