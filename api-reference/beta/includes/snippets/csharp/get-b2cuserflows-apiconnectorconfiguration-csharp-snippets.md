---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9e864b224c670dc427e3ee1c9153d464b6ee50fa
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63332407"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var b2cUserFlows = await graphClient.Identity.B2cUserFlows["{b2cIdentityUserFlow-id}"]
    .Request()
    .Expand("postFederationSignup,postAttributeCollection")
    .Select("ApiConnectorConfiguration")
    .GetAsync();

var apiConnectorConfiguration = b2cUserFlows.ApiConnectorConfiguration;

```