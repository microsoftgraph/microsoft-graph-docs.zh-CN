---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c64d16b6bed0d40c7ac38ca37be5acec3ebc18a8
ms.sourcegitcommit: 64d27a0e3dcccc9d857e62aace4153e5d98fb3d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60730198"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("expand", "submissions")
};

var assignments = await graphClient.Education.Users["{educationUser-id}"].Assignments
    .Request( queryOptions )
    .GetAsync();

```