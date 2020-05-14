---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 01cd8bf458094a1febdfc3cc31abc595fc7e6630
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2020
ms.locfileid: "44218245"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workforceIntegration = new WorkforceIntegration
{
    DisplayName = "displayName-value",
    ApiVersion = 99,
    Encryption = new WorkforceIntegrationEncryption
    {
        Protocol = WorkforceIntegrationEncryptionProtocol.SharedSecret,
        Secret = "secret-value"
    },
    IsActive = true,
    Url = "url-value",
    SupportedEntities = WorkforceIntegrationSupportedEntities.None
};

await graphClient.Teamwork.WorkforceIntegrations
    .Request()
    .AddAsync(workforceIntegration);

```