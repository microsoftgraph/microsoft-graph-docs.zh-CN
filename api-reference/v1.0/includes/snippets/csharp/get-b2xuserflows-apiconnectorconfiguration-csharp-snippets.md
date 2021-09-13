---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 63e6fa6580873c08b80be5baa96d76b74511e50e21bd6c37721fe91ffe8e7624
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332151"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var b2xUserFlows = await graphClient.Identity.B2xUserFlows["{b2xIdentityUserFlow-id}"]
    .Request()
    .Expand("postAttributeCollection")
    .Select("ApiConnectorConfiguration")
    .GetAsync();

var apiConnectorConfiguration = b2xUserFlows.ApiConnectorConfiguration;

```