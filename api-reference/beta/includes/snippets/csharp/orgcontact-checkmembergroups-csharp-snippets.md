---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 19e7f26a82c30f51364534dfe768f5ec2e981ceb
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48618028"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var groupIds = new List<String>()
{
    "groupIds-value"
};

await graphClient.Contacts["{id}"]
    .CheckMemberGroups(groupIds)
    .Request()
    .PostAsync();

```