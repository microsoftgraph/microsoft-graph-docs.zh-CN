---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 33cb6e273c28aeb549ba88cfce8433a6e9eaf64e
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48603609"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var groups = await graphClient.Groups
    .Request()
    .GetAsync();

```