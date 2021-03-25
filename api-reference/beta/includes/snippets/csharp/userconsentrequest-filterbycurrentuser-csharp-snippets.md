---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0a85ffff3d79922d69338ea932b8d636f7a958da
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51201860"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var userConsentRequest = await graphClient.IdentityGovernance.AppConsent.AppConsentRequests["{appConsentRequest-id}"].UserConsentRequests["{userConsentRequest-id}"]
    .Request()
    .Filter(" (status eq 'Completed')")
    .GetAsync();

```