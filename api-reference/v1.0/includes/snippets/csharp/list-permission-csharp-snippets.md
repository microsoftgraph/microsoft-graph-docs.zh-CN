---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 461168e811bc204d0eb0caa8ab4a51dcfbc07f2c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50791246"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var permissions = await graphClient.Sites["{site-id}"].Permissions
    .Request()
    .GetAsync();

```