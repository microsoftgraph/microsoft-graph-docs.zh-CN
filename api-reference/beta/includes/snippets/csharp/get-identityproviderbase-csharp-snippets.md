---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1e116fd2e1e3a6445bac061a3c13918cf3fdeac069188865224790d1839192b2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56904248"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var identityProviders = await graphClient.Identity.IdentityProviders
    .Request()
    .GetAsync();

```