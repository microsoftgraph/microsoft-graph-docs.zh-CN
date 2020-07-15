---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 335f5de25968f8c8392f9a61ed458f2c41354e1a
ms.sourcegitcommit: 2c8a12389b82ee5101b2bd17eae11b42e65e52c0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2020
ms.locfileid: "45142325"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var application = new Application
{
    OnPremisesPublishing = new OnPremisesPublishing
    {
        SingleSignOnSettings = new OnPremisesPublishingSingleSignOn
        {
            KerberosSignOnSettings = new KerberosSignOnSettings
            {
                KerberosServicePrincipalName = "HTTP/iwademo.contoso.com",
                KerberosSignOnMappingAttributeType = KerberosSignOnMappingAttributeType.UserPrincipalName
            },
            SingleSignOnMode = SingleSignOnMode.OnPremisesKerberos
        }
    }
};

await graphClient.Applications["bf21f7e9-9d25-4da2-82ab-7fdd85049f83"]
    .Request()
    .UpdateAsync(application);

```