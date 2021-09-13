---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 47a1c22a34aca8d714df561e01f62843829a6dd6ac86315101dea7d49255a800
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279314"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var filterByCurrentUser = await graphClient.IdentityGovernance.AppConsent.AppConsentRequests["{appConsentRequest-id}"].UserConsentRequests
    .FilterByCurrentUser(ConsentRequestFilterByCurrentUserOptions.Reviewer)
    .Request()
    .Filter(" (status eq 'Completed')")
    .GetAsync();

```