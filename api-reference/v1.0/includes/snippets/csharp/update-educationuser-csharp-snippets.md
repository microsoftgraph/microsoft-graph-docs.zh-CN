---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 41f51ceabb94be4aa2e2474f7fe7ef232f9cae76
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50805791"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationUser = new EducationUser
{
    DisplayName = "Rogelio Cazares",
    GivenName = "Rogelio",
    MiddleName = "Fernando",
    Surname = "Cazares"
};

await graphClient.Education.Users["{educationUser-id}"]
    .Request()
    .UpdateAsync(educationUser);

```