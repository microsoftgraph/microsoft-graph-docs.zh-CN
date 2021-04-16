---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a8b3aaf7c0efb3e87733727a17896480fbae41a4
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2021
ms.locfileid: "51837877"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var filterByCurrentUser = await graphClient.IdentityGovernance.AppConsent.AppConsentRequests
    .FilterByCurrentUser(ConsentRequestFilterByCurrentUserOptions.Reviewer)
    .Request()
    .Filter("userConsentRequests/any(u:u/status eq 'InProgress')")
    .GetAsync();

```