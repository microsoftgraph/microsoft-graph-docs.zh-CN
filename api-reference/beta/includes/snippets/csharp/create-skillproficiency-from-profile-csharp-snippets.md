---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dde9eaef6c5d4acffb1ab76a86906a683596785e
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/20/2020
ms.locfileid: "46821271"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var skillProficiency = new SkillProficiency
{
    Categories = new List<String>()
    {
        "Professional"
    },
    AllowedAudiences = AllowedAudiences.Organization,
    DisplayName = "API Design",
    Proficiency = SkillProficiencyLevel.GeneralProfessional,
    CollaborationTags = new List<String>()
    {
        "ableToMentor"
    }
};

await graphClient.Me.Profile.Skills
    .Request()
    .AddAsync(skillProficiency);

```