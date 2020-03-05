---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 90fb74c7de8da2c7aeff452d60d145cfa8c57ae6
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "37996552"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var languageProficiency = new LanguageProficiency
{
    DisplayName = "displayName-value",
    Tag = "tag-value",
    Proficiency = LanguageProficiencyLevel.Elementary
};

await graphClient.Me.Profile.Languages
    .Request()
    .AddAsync(languageProficiency);

```