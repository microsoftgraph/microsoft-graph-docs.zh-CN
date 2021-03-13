---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fd353ed8bd8247b773c46e65b5d58ca8fc604cfc
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50802121"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryRole = await graphClient.DirectoryRoles["{directoryRole-id}"]
    .Request()
    .GetAsync();

```