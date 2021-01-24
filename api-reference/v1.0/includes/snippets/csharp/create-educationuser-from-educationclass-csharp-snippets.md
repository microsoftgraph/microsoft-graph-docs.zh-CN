---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 35f80492c0e32dd9c7b91fa05f1207310696085a
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2021
ms.locfileid: "49944895"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationUser = new EducationUser
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"@odata.id", "https://graph.microsoft.com/v1.0/education/users/13015"}
    }
};

await graphClient.Education.Classes["{class-id}"].Members.References
    .Request()
    .AddAsync(educationUser);

```