---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 042e44538f045a9329cce09bf2c84b10b196a300
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50786122"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Sites["{site-id}"].Permissions["{permission-id}"]
    .Request()
    .DeleteAsync();

```