---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ed4d8090979a4ed065f55ec528973665b4f12706
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/30/2021
ms.locfileid: "61225002"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var groupIds = new List<String>()
{
    "f448435d-3ca7-4073-8152-a1fd73c0fd09",
    "bd7c6263-4dd5-4ae8-8c96-556e1c0bece6",
    "93670da6-d731-4366-94b5-abed40b6016b",
    "f5484ab1-4d4d-41ec-a9b8-754b3957bfc7",
    "c9103f26-f3cf-4004-a611-2a14e81b8f79"
};

await graphClient.DirectoryObjects["{directoryObject-id}"]
    .CheckMemberGroups(groupIds)
    .Request()
    .PostAsync();

```