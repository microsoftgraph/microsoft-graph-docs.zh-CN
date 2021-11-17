---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 44a0b7f3fe98fcece400790c1da08b4188fd12e5904931aa93c2f10e527e8463
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104653"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var overridesPages = await graphClient.Identity.B2cUserFlows["{b2cIdentityUserFlow-id}"].Languages["{userFlowLanguageConfiguration-id}"].OverridesPages
    .Request()
    .GetAsync();

```