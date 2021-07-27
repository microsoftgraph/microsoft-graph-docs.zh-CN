---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e628845ad059bff51c62d06e9ba73c0d357403d4
ms.sourcegitcommit: 5bb981b4853663354a566d4a4a5cbf288939e441
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2021
ms.locfileid: "53579789"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var identityProviders = await graphClient.Identity.IdentityProviders
    .Request()
    .GetAsync();

```