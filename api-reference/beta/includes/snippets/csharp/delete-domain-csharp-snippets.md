---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eb143d00ead236726b37b1e8f2d29d4106a1d476
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48617429"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Domains["contoso.com"]
    .Request()
    .DeleteAsync();

```