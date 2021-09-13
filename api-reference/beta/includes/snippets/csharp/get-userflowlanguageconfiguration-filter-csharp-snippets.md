---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 44af0f3f6926f69652a07fce10b5262d88bd291c5f54e675918a82728426a1e4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215924"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var languages = await graphClient.Identity.B2cUserFlows["{b2cIdentityUserFlow-id}"].Languages
    .Request()
    .Filter("isEnabled eq true")
    .GetAsync();

```