---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 1c99fbc336310bf44f23fcfabdf4f187946727bf
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34448969"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var memberOf = await graphClient.Contacts["{id}"].MemberOf
    .Request()
    .GetAsync();

```