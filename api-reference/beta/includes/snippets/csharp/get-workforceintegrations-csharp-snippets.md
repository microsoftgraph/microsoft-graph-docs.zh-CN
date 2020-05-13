---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a46b15c50afc17fba647ca0c7dd8168d354739d3
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2020
ms.locfileid: "40870576"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workforceIntegrations = await graphClient.Teamwork.WorkforceIntegrations
    .Request()
    .GetAsync();

```