---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 0c2ef9fb22dbd6ba3accd317714066f9ae2f8e38
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35520598"
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

await graphClient.Education.Users["13020"]
    .Request()
    .UpdateAsync(educationUser);

```