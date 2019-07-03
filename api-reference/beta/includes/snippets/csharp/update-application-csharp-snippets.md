---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 66b16f590e48ee5c9c9bce0b5f79174eae968390
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35478600"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var application = new Application
{
    AllowPublicClient = false,
    DisplayName = "New display name"
};

await graphClient.Applications["{id}"]
    .Request()
    .UpdateAsync(application);

```