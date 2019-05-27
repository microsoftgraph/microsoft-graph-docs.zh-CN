---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 17f2500e14b0cbf0f0a52804fdb573ebdd85c97b
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34480999"
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