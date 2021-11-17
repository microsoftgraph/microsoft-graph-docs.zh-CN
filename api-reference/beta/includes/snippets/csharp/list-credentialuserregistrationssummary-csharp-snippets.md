---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7b3d25d63822f504c5cd6efb29d59dbbcf4b803082bb6c866a1ee4ebba72b00f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278078"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var credentialUserRegistrationsSummaries = await graphClient.TenantRelationships.ManagedTenants.CredentialUserRegistrationsSummaries
    .Request()
    .GetAsync();

```