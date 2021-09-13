---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5813b383361711ceddb27414c47f088008023f48dcb22db6ab5bb1916c6c418e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105568"
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