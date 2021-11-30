---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 468acfbba646cb6ff0a9dad6c6731b64901529fa
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/30/2021
ms.locfileid: "61226207"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var servicePrincipal = new ServicePrincipal
{
    CustomSecurityAttributes = new CustomSecurityAttributeValue
    {
        AdditionalData = new Dictionary<string, object>()
        {
            {"Engineering", "{\"@odata.type\":\"#Microsoft.DirectoryServices.CustomSecurityAttributeValue\",\"ProjectDate\":\"2022-10-01\"}"}
        }
    }
};

await graphClient.ServicePrincipals["{servicePrincipal-id}"]
    .Request()
    .UpdateAsync(servicePrincipal);

```