---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3633fb1f4ee3d811cb0f20d761260b17adbc7a1d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50961038"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var identityProvider = await graphClient.IdentityProviders["{identityProvider-id}"]
    .Request()
    .GetAsync();

```