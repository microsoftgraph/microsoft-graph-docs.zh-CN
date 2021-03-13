---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4c237761df6bc7d9f0e132fde15b551d0668f221
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50805638"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = await graphClient.DirectoryObjects["{directoryObject-id}"]
    .Request()
    .Filter("isOf('Microsoft.Graph.User') or isOf('Microsoft.Graph.Group')")
    .GetAsync();

```