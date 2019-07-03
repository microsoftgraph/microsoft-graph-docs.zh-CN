---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 6deea81809038243dba78fcaae14a82900e00dd4
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35480065"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var groupLifecyclePolicies = await graphClient.Groups["{id}"].GroupLifecyclePolicies
    .Request()
    .GetAsync();

```