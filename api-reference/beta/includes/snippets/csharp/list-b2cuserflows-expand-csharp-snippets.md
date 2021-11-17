---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d489bf4d0ecc46768114953d6276e9df48def7ac7968e844a2b853574b417c60
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163815"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var b2cUserFlows = await graphClient.Identity.B2cUserFlows
    .Request()
    .Expand("identityProviders")
    .GetAsync();

```