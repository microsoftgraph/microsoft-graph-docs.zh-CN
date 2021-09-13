---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3b8695bf4687f7c862d8bccc05b25ec204aebcd5d254c5985157438b72d9802e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104991"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationClass = new EducationClass
{
    DisplayName = "String",
    MailNickname = "String",
    Description = "String",
    CreatedBy = new IdentitySet
    {
    },
    ClassCode = "String",
    ExternalName = "String",
    ExternalId = "String",
    ExternalSource = EducationExternalSource.Sis,
    ExternalSourceDetail = "String",
    Grade = "String",
    Term = new EducationTerm
    {
    }
};

await graphClient.Education.Classes
    .Request()
    .AddAsync(educationClass);

```