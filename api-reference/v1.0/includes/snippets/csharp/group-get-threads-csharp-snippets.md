---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 184fc578e63f2d236df4ab7b9ef75cc7fd4e840c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50780058"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var threads = await graphClient.Groups["{group-id}"].Threads
    .Request()
    .GetAsync();

```