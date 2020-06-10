---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eb368dc1d71959e0556e2d9ea63330c6729ee8c9
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44684714"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var group = await graphClient.Users["{id}"].TransitiveMemberOf
    .Request()
    .Header("ConsistencyLevel","eventual")
    .Search("displayName:tier")
    .Select("displayName,id")
    .OrderBy("displayName ")
    .GetAsync();

```