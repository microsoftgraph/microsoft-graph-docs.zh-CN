---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5596afda4e06f50786dec069da665572f1cb465a73f8fa317f9643e870b6bd97
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104859"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.IdentityGovernance.EntitlementManagement.ConnectedOrganizations["{connectedOrganization-id}"]
    .Request()
    .DeleteAsync();

```