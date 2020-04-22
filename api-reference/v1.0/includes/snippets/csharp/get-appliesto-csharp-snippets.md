---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6af7a3931b36dfbb2f11e65a44f0781f3502ed57
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43718642"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var appliesTo = await graphClient.Policies.TokenLifetimePolicies["{id}"].AppliesTo
    .Request()
    .GetAsync();

```