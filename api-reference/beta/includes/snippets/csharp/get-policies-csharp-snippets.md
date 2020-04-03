---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3ab2c63a5ac4de242987e5ba7f58079564ec1a46
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/03/2020
ms.locfileid: "43127103"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var policies = await graphClient.Identity.ConditionalAccess.Policies
    .Request()
    .Filter("displayName eq 'SimplePolicy1' or displayName eq 'SimplePolicy2'")
    .GetAsync();

```