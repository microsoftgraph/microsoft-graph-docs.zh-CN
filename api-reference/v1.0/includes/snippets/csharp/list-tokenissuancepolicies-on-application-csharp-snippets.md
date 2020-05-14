---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6dd7eb02e15c79e8b65c2d442d70dc3f5cef554c
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2020
ms.locfileid: "43510524"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tokenIssuancePolicies = await graphClient.Applications["{id}"].TokenIssuancePolicies
    .Request()
    .GetAsync();

```