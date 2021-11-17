---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e42769c71d83bb6096b2681eaf7b1eb7d2b996702fd42cf07e4f527e46ee90d6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105139"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var languageProficiency = new LanguageProficiency
{
    AllowedAudiences = AllowedAudiences.Organization
};

await graphClient.Me.Profile.Languages["{languageProficiency-id}"]
    .Request()
    .UpdateAsync(languageProficiency);

```