---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 17f2500e14b0cbf0f0a52804fdb573ebdd85c97b
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48605663"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationClass = new EducationClass
{
    Description = "Health Level 1",
    ClassCode = "Health 501",
    DisplayName = "Health 1",
    ExternalId = "11019",
    ExternalName = "Health Level 1",
    ExternalSource = EducationExternalSource.Sis,
    MailNickname = "fineartschool.net"
};

await graphClient.Education.Classes
    .Request()
    .AddAsync(educationClass);

```