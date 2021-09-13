---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6e40d719a6f6f7fd6cd78393760e7892b6601226cee6a19a1894d512c9ba2009
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215905"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var userFlowLanguageConfiguration = new UserFlowLanguageConfiguration
{
    Id = "es-ES",
    IsEnabled = true
};

await graphClient.Identity.B2cUserFlows["{b2cIdentityUserFlow-id}"].Languages["{userFlowLanguageConfiguration-id}"]
    .Request()
    .PutAsync(userFlowLanguageConfiguration);

```