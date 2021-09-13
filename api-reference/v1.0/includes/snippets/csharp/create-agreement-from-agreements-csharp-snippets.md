---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e993a93e301d03a1a9670c6690af9f9661bb28898c6c2449658e2bc2bccccc66
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279425"
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
                Data = Encoding.ASCII.GetBytes("SGVsbG8gd29ybGQ=")
            }
        }
    }
};

await graphClient.IdentityGovernance.TermsOfUse.Agreements
    .Request()
    .AddAsync(agreement);

```