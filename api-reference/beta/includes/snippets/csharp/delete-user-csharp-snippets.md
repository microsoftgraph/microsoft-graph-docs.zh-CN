---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 259990ecc632f46d65d5cf7f96bad6ab19d18202
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48613839"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Users["ba9a3254-9f18-4209-aeb3-9e42a35b5be4"]
    .Request()
    .DeleteAsync();

```