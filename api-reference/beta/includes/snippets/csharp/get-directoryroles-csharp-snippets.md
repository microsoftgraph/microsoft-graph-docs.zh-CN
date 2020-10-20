---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 80be132d0345accb780d2c9c1ddee8a6d9b9fb4e
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48613757"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryRoles = await graphClient.DirectoryRoles
    .Request()
    .GetAsync();

```