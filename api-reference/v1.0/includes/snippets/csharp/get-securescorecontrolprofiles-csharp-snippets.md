---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 93ce8a44569ca6bff742900572eb9b3e99b28ff2
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35735818"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var secureScoreControlProfiles = await graphClient.Security.SecureScoreControlProfiles
    .Request()
    .GetAsync();

```