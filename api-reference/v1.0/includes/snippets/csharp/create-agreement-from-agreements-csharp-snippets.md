---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 41e8ea251511ed1bb8a33225ec65451c9e529793
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60988699"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var agreement = new Agreement
{
    DisplayName = "MSGraph Sample",
    IsViewingBeforeAcceptanceRequired = true,
    Files = new AgreementFilesCollectionPage()
    {
        new AgreementFileLocalization
        {
            FileName = "TOU.pdf",
            Language = "en",
            IsDefault = true,
            FileData = new AgreementFileData
            {
                Data = Convert.FromBase64String("SGVsbG8gd29ybGQ=")
            }
        }
    }
};

await graphClient.IdentityGovernance.TermsOfUse.Agreements
    .Request()
    .AddAsync(agreement);

```