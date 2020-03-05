---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bc5297566e7267f68368b6ada43c3c7f9dd2d1d3
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "37997757"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var skillProficiency = new SkillProficiency
{
    Categories = new List<String>()
    {
        "categories-value"
    },
    DisplayName = "displayName-value",
    Proficiency = SkillProficiencyLevel.Elementary,
    WebUrl = "webUrl-value"
};

await graphClient.Me.Profile.Skills
    .Request()
    .AddAsync(skillProficiency);

```