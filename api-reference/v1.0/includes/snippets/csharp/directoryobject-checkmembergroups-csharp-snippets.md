---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7948c093c672d2c4d2c02a2aca4fe007a81531ae
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48608849"
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