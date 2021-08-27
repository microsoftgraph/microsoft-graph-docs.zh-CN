---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 06fd392a3310066cdd3115ff20a3f62aca191911d67b6d98a14cc837297c79ad
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106901"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var availableProviderTypes = await graphClient.Identity.IdentityProviders
    .AvailableProviderTypes()
    .Request()
    .GetAsync();

```