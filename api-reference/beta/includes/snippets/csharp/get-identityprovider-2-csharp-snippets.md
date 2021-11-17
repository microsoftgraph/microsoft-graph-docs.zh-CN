---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2ec0646430495cae9de507c68bbdb634e0580f78bce8c6c5fb8af5b1ae431099
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219199"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var identityProvider = await graphClient.IdentityProviders["{identityProvider-id}"]
    .Request()
    .GetAsync();

```