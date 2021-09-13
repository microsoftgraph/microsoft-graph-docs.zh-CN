---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5675ea8b1234c2ae6291226199e2bb03e2f9e9f422815d229702d3b53eaa66b5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332842"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var policies = await graphClient.TrustFramework.Policies
    .Request()
    .GetAsync();

```