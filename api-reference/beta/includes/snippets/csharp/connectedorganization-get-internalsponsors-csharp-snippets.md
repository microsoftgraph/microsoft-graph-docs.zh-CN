---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6d1684154471c47aaf82a2754d660e72212c0944b6d47c9169f5375c0b40bad7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104846"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var internalSponsors = await graphClient.IdentityGovernance.EntitlementManagement.ConnectedOrganizations["{connectedOrganization-id}"].InternalSponsors
    .Request()
    .GetAsync();

```