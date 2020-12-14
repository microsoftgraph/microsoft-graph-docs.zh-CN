---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cdee97da65b438e57cd71c0fb71388594932966d
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/11/2020
ms.locfileid: "49659001"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var userSource = new UserSource
{
    Email = "megan@contoso.com",
    IncludedSources = SourceType.Mailbox | SourceType.Site
};

await graphClient.Compliance.Ediscovery.Cases["4c8f8f70-7785-4bd4-b296-c98376a2c5e1"].Custodians["2192ca408ea2410eba3bec8ae873be6b"].UserSources
    .Request()
    .AddAsync(userSource);

```