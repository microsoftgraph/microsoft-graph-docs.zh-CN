---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d8f7252ebe32a019b1b7a52705c8ab79104f9255
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/16/2022
ms.locfileid: "63528185"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var agreement = new Agreement
{
    DisplayName = "Contoso ToU for guest users",
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
                Data = Convert.FromBase64String("SGVsbG8gd29ybGQ=//truncated-binary")
            }
        }
    }
};

await graphClient.IdentityGovernance.TermsOfUse.Agreements
    .Request()
    .AddAsync(agreement);

```