---
description: 自动生成的文件。 不修改
ms.openlocfilehash: fefe19a5b855651cda487edbeb0738f4817e5e39
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34470471"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = new DirectoryObject
{
};

await graphClient.Users["{id}"].Manager
    .Request()
    .PutAsync(directoryObject);

```