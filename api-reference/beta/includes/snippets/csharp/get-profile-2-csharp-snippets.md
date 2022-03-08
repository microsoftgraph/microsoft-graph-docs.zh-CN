---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fd343314fd381cd264eedfa17cdf4e1946bfa3af
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63351189"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var profile = await graphClient.Me.Profile
    .Request()
    .Expand("names($select=first,last),skills($select=displayName)")
    .GetAsync();

```