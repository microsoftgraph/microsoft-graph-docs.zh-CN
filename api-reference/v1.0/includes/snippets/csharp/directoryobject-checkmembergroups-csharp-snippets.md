---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 42049d1d901b41d90221486a21a2f5a79255ff3b896880ff841dceffb2a598bb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903359"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var groupIds = new List<String>()
{
    "fee2c45b-915a-4a64b130f4eb9e75525e",
    "4fe90ae065a-478b9400e0a0e1cbd540"
};

await graphClient.DirectoryObjects["{directoryObject-id}"]
    .CheckMemberGroups(groupIds)
    .Request()
    .PostAsync();

```