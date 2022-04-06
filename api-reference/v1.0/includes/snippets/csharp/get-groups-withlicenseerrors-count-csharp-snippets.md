---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2b49bbd16f464300c1e54be5df39cb8f8583fa47
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/16/2022
ms.locfileid: "63528126"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("$count", "true")
};

var groups = await graphClient.Groups
    .Request( queryOptions )
    .Header("ConsistencyLevel","eventual")
    .Filter("hasMembersWithLicenseErrors eq true")
    .Select("id,displayName")
    .GetAsync();

```