---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a3c840c973eb41db23b6d0da5c6799651541087e
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46570107"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var agreement = new Agreement
{
    DisplayName = "MSGraph Sample",
    IsViewingBeforeAcceptanceRequired = true,
    Files = (IAgreementFilesCollectionPage)new List<AgreementFileLocalization>()
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

await graphClient.Agreements
    .Request()
    .AddAsync(agreement);

```