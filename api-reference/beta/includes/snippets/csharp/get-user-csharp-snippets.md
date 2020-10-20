---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: df033299fdf749885fa325181e5184f66d0d740a
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48613072"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var user = await graphClient.Me
    .Request()
    .GetAsync();

```