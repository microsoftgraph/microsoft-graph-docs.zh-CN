---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 77981e93f43fc4cf9a0a0fcdd94fc268524b8cb2
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35467814"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Domains["{domain-name}"]
    .Verify()
    .Request()
    .PostAsync();

```