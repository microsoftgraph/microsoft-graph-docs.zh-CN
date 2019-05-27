---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 7948c093c672d2c4d2c02a2aca4fe007a81531ae
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34458118"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var groupIds = new List<String>()
{
    "fee2c45b-915a-4a64b130f4eb9e75525e",
    "4fe90ae065a-478b9400e0a0e1cbd540"
};

await graphClient.DirectoryObjects["{id}"]
    .CheckMemberGroups(groupIds)
    .Request()
    .PostAsync();

```