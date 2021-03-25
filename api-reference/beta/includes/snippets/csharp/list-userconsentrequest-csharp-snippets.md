---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4acfc3282ff104ed0e0ba4a3cfac6365e8b1c0c8
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51201824"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var userConsentRequests = await graphClient.IdentityGovernance.AppConsent.AppConsentRequests["{appConsentRequest-id}"].UserConsentRequests
    .Request()
    .GetAsync();

```