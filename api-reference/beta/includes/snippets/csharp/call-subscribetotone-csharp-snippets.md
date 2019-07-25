---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9d1eaa527b5cb9dca4e60e00e8f94ad1708aa5e6
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35708810"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var clientContext = "d45324c1-fcb5-430a-902c-f20af696537c";

await graphClient.App.Calls["{id}"]
    .SubscribeToTone(clientContext)
    .Request()
    .PostAsync();

```