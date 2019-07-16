---
description: 自动生成的文件。 不修改
ms.openlocfilehash: aa38368f00ba725d180f9c4d6e7a6b93c7570795
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35740305"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var message = new Message
{
    IsRead = "true"
};

await graphClient.Me.Messages["{id}"]
    .Request()
    .UpdateAsync(message);

```