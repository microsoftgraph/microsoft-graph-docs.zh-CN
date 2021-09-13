---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 95f7a9d34c0ba3d652afa0334472e4f8458d7d5a4b269d030d34be64a6040232
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57164223"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var overridesPages = await graphClient.Identity.B2xUserFlows["{b2xIdentityUserFlow-id}"].Languages["{userFlowLanguageConfiguration-id}"].OverridesPages
    .Request()
    .GetAsync();

```