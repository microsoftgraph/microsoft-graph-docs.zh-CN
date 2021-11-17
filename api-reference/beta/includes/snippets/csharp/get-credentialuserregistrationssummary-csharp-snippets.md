---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8bbcd0d8c2e95d15fba6dac06fba6e512dab0eec1acb110f0783cb59f295cfbc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278291"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var credentialUserRegistrationsSummary = await graphClient.TenantRelationships.ManagedTenants.CredentialUserRegistrationsSummaries["{managedTenants.credentialUserRegistrationsSummary-id}"]
    .Request()
    .GetAsync();

```