---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 85e353c496711d52e7070718e10f23d3d205bdd7faecfb8ff9c1df46aa7285a5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163996"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationUser = new EducationUser
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"@odata.id", "https://graph.microsoft.com/beta/education/users/14011"}
    }
};

await graphClient.Education.Classes["{educationClass-id}"].Teachers.References
    .Request()
    .AddAsync(educationUser);

```