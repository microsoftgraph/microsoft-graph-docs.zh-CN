---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1c3e21c635a6b53e76540a59b42c32f0c697bfaf6dd1c5cb48689b0ba166284f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332430"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var b2xIdentityUserFlow = new B2xIdentityUserFlow
{
    Id = "UserFlowWithAPIConnector",
    UserFlowType = UserFlowType.SignUpOrSignIn,
    UserFlowTypeVersion = 1f,
    ApiConnectorConfiguration = new UserFlowApiConnectorConfiguration
    {
        PostFederationSignup = new IdentityApiConnector
        {
            AdditionalData = new Dictionary<string, object>()
            {
                {"@odata.id", "https://graph.microsoft.com/v1/identity/apiConnectors/{id}"}
            }
        },
        PostAttributeCollection = new IdentityApiConnector
        {
            AdditionalData = new Dictionary<string, object>()
            {
                {"@odata.id", "https://graph.microsoft.com/v1/identity/apiConnectors/{id}"}
            }
        }
    }
};

await graphClient.Identity.B2xUserFlows
    .Request()
    .AddAsync(b2xIdentityUserFlow);

```