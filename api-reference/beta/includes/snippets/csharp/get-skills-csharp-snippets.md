---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b28b6d3eed5a2db857233efe422503da8d2492ab
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "37997900"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var skills = await graphClient.Me.Profile.Skills
    .Request()
    .GetAsync();

```