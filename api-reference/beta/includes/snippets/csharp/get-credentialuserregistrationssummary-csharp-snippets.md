---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4ad97c2c6e608e9a8697fb5bca22e8fdaf225aea
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440016"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var credentialUserRegistrationsSummary = await graphClient.TenantRelationships.ManagedTenants.CredentialUserRegistrationsSummaries["{managedTenants.credentialUserRegistrationsSummary-id}"]
    .Request()
    .GetAsync();

```