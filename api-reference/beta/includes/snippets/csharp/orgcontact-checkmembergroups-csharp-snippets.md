---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 19e7f26a82c30f51364534dfe768f5ec2e981ceb
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35721089"
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