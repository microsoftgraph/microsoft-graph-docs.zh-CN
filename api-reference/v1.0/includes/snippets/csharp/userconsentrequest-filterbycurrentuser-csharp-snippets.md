---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bd25a277732e1223aeec4883e6a928ec986d4cda
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51507990"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var filterByCurrentUser = await graphClient.IdentityGovernance.AppConsent.AppConsentRequests["{appConsentRequest-id}"].UserConsentRequests
    .FilterByCurrentUser(On.Reviewer)
    .Request()
    .Filter(" (status eq 'Completed')")
    .GetAsync();

```