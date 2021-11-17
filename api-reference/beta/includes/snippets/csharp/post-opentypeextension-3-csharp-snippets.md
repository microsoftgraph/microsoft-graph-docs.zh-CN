---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e3149c912dfd01ee4349bca4fdde27df1c966fd78573237a31be067bcee1843e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221367"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var extension = new OpenTypeExtension
{
    ExtensionName = "Com.Contoso.Deal",
    AdditionalData = new Dictionary<string, object>()
    {
        {"companyName", "Alpine Skis"},
        {"dealValue", "1010100"},
        {"expirationDate", "2015-07-03T13:04:00Z"}
    }
};

await graphClient.Groups["{group-id}"].Events["{event-id}"].Extensions
    .Request()
    .AddAsync(extension);

```