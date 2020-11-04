---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eb368dc1d71959e0556e2d9ea63330c6729ee8c9
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48904294"
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