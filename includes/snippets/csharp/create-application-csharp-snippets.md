---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2d7adfb56620cffe488409da4b2260e87d3bf36e
ms.sourcegitcommit: ef47b165f7a140cfc0309a275cb8722dd265660d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2020
ms.locfileid: "48373297"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var application = new Application
{
    DisplayName = "Contoso IWA App",
    SignInAudience = "AzureADMyOrg"
};

await graphClient.Applications
    .Request()
    .AddAsync(application);

```