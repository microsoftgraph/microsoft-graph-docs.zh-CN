---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6fd649462da4d0e78a4ae8403ccc884557893bdb1a1fa53172a3ccc55be1da55
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278953"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var identityProviderBase = await graphClient.Identity.IdentityProviders["{identityProviderBase-id}"]
    .Request()
    .GetAsync();

```