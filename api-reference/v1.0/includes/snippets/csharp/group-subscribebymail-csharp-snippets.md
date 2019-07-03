---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 77ee4b7f593abf745654a2c7605e135c4e260fc2
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35467725"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Groups["{id}"]
    .SubscribeByMail()
    .Request()
    .PostAsync();

```