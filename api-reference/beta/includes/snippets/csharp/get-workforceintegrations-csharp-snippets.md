---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a46b15c50afc17fba647ca0c7dd8168d354739d3
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2020
ms.locfileid: "40870576"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workforceIntegrations = await graphClient.Teamwork.WorkforceIntegrations
    .Request()
    .GetAsync();

```