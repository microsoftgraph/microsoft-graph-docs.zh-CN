---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 660a6092e05e29f87055d69c9c04f57f6f3e8dbb
ms.sourcegitcommit: 1d9193fa91f44d80ecdc2b82e37272df1c9630f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/22/2022
ms.locfileid: "65629227"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var agreementFileLocalization = new AgreementFileLocalization
{
    FileName = "Contoso ToU for guest users (French)",
    Language = "fr-FR",
    IsDefault = false,
    IsMajorVersion = false,
    DisplayName = "Contoso ToU for guest users (French)",
    FileData = new AgreementFileData
    {
        Data = Convert.FromBase64String("base64JVBERi0xLjUKJb/3ov4KNCAwIG9iago8PCAvTGluZWFyaX//truncated-binary-data")
    }
};

await graphClient.IdentityGovernance.TermsOfUse.Agreements["{agreement-id}"].Files
    .Request()
    .AddAsync(agreementFileLocalization);

```