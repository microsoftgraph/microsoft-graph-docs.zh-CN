---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3dd37bfe6667ef4180b565901f051ee9ec171e2d
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48905859"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var int32 = await graphClient.Users["{id}"].MemberOf.$count
    .Request()
    .Header("ConsistencyLevel","eventual")
    .GetAsync();

```