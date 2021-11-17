---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 03aee4820528baf962b88e9045774d4131abbb569138656f546c45ac856d62c6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104840"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var connectedOrganizations = await graphClient.IdentityGovernance.EntitlementManagement.ConnectedOrganizations
    .Request()
    .GetAsync();

```