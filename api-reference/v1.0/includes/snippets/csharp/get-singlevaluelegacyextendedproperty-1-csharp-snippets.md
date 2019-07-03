---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 139fa80f71538c1c3bce37102beba299e7e06a2d
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35493689"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var message = await graphClient.Me.Messages["AAMkAGE1M2_bs88AACHsLqWAAA="]
    .Request()
    .Filter("id eq 'String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color')")
    .Expand("singleValueExtendedProperties($filter=id%20eq%20'String%20%7B66f5a359-4659-4830-9070-00047ec6ac6e%7D%20Name%20Color')")
    .GetAsync();

```