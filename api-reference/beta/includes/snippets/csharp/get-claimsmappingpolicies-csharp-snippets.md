---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 83c120cd81dfa9be46418ac2e388ec98af5e8252
ms.sourcegitcommit: 2f78ac96a9b0462626a242429055ef824590bd3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2020
ms.locfileid: "41476366"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var policy = await graphClient.Policies["claimsMappingPolicies"]
    .Request()
    .GetAsync();

```