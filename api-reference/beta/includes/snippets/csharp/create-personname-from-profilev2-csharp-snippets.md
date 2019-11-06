---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f95ebaf0bb7dec1102a7f795198845e0b3d4afe2
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37997788"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var personName = new PersonName
{
    DisplayName = "displayName-value",
    First = "first-value",
    Initials = "initials-value",
    Last = "last-value",
    LanguageTag = "languageTag-value",
    Maiden = "maiden-value"
};

await graphClient.Me.Profile.Names
    .Request()
    .AddAsync(personName);

```