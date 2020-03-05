---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3ef64f13d9022edd0460f133fd323b04600226e5
ms.sourcegitcommit: 2f78ac96a9b0462626a242429055ef824590bd3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2020
ms.locfileid: "41558915"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var policy = await graphClient.Policies["tokenLifetimePolicies"]
    .Request()
    .GetAsync();

```