---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c898fc569ac4e220eab07cd320a721e21cb6a550
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50946052"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var appRoleAssignment = new AppRoleAssignment
{
    PrincipalId = Guid.Parse("7679d9a4-2323-44cd-b5c2-673ec88d8b12"),
    ResourceId = Guid.Parse("076e8b57-bac8-49d7-9396-e3449b685055"),
    AppRoleId = Guid.Parse("00000000-0000-0000-0000-000000000000")
};

await graphClient.Groups["{group-id}"].AppRoleAssignments
    .Request()
    .AddAsync(appRoleAssignment);

```