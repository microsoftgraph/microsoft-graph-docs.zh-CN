---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 05c72b41873711a44904c306761e4b9f44cb0f71
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51201894"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var userConsentRequest = await graphClient.IdentityGovernance.AppConsent.AppConsentRequests["{appConsentRequest-id}"].UserConsentRequests["{userConsentRequest-id}"]
    .Request()
    .GetAsync();

```