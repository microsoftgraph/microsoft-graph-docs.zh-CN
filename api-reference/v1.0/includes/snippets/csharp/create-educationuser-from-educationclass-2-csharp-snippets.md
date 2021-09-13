---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ec712b46a9f02810204c42691daf2c6ffb5633b5a46714d74b5c7a2019302fe3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409572"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationUser = new EducationUser
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"@odata.id", "https://graph.microsoft.com/v1.0/education/users/14011"}
    }
};

await graphClient.Education.Classes["{educationClass-id}"].Teachers.References
    .Request()
    .AddAsync(educationUser);

```