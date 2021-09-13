---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 85c41a3f7a0ca5fc8da0a1ac0ea048087ab9b1dbf3193f895bf9e67f714d73cb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279241"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Identity.B2cUserFlows["{b2cIdentityUserFlow-id}"].Languages["{userFlowLanguageConfiguration-id}"].OverridesPages["{userFlowLanguagePage-id}"].Content
    .Request()
    .DeleteAsync();

```