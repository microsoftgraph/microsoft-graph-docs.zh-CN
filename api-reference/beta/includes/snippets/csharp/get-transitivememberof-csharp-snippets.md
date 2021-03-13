---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fbd2afbd3faf1ab09cbe7398892a3e8637182176
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50806132"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var transitiveMemberOf = await graphClient.Users["{user-id}"].TransitiveMemberOf
    .Request()
    .GetAsync();

```