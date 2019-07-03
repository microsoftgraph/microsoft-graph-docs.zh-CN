---
description: 自动生成的文件。 不修改
ms.openlocfilehash: fd9e920f849acb8299eb59db38d24b66e59e555b
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35478316"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = await graphClient.DirectoryObjects["delta"]
    .Request()
    .Filter("isOf('Microsoft.Graph.User')+or+isOf('Microsoft.Graph.Group')")
    .GetAsync();

```