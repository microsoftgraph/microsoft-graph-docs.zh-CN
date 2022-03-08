---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aa99d3f7b301c92f17d3c7306c2874152abb2813
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63332288"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var b2xUserFlows = await graphClient.Identity.B2xUserFlows["{b2xIdentityUserFlow-id}"]
    .Request()
    .Expand("postFederationSignup,postAttributeCollection")
    .Select("ApiConnectorConfiguration")
    .GetAsync();

var apiConnectorConfiguration = b2xUserFlows.ApiConnectorConfiguration;

```