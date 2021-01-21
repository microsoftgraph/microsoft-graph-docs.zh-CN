---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 32792408cf04885a754bb3d68052027ebd8ed2e7
ms.sourcegitcommit: 6314172db76ba9f2c192d8c099d818c5e772d2b8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2021
ms.locfileid: "49910505"
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

await graphClient.Teamwork.WorkforceIntegrations["{workforceIntegrationId}"]
    .Request()
    .UpdateAsync(workforceIntegration);

```