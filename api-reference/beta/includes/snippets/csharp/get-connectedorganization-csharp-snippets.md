---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dfa958476a548e9547f37c3640747b1645a8d93b6bda4beb7992da805c6edaf9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104856"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var connectedOrganization = await graphClient.IdentityGovernance.EntitlementManagement.ConnectedOrganizations["{connectedOrganization-id}"]
    .Request()
    .GetAsync();

```