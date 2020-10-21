---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 77981e93f43fc4cf9a0a0fcdd94fc268524b8cb2
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48621960"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Domains["{domain-name}"]
    .Verify()
    .Request()
    .PostAsync();

```