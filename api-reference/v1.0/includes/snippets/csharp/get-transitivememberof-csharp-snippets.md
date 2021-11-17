---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f8e6cd2933ff8b54f9a3fb2e355e84631a9e98abcdfb131efcb99c1ff4f17a5f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162531"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var transitiveMemberOf = await graphClient.Users["{user-id}"].TransitiveMemberOf
    .Request()
    .GetAsync();

```