---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 030ab885b4c201cd967d7b098457b25e627c7b6e
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "49689160"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var ids = new List<String>()
{
    "fa8bf3dc-eca7-46b7-bad1-db199b62afc3",
    "66825e03-7ef5-42da-9069-724602c31f6b"
};

await graphClient.Communications
    .GetPresencesByUserId(ids)
    .Request()
    .PostAsync();

```