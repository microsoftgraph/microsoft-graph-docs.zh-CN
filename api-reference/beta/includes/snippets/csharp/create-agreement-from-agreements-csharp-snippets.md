---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e920f031cd35a5b19a8842f858a003489fd01cb3
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2021
ms.locfileid: "49945793"
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

await graphClient.Agreements
    .Request()
    .AddAsync(agreement);

```