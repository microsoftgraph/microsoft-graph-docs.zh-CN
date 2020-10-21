---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 383a6f633a95290ce91ad57573c489c2a3a2b512
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48622088"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var transitiveMemberOf = await graphClient.Me.TransitiveMemberOf
    .Request()
    .GetAsync();

```