---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7095677e1dcfe729bfeb16cb67696ccf0abab8d1
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50793731"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delegatedPermissionClassification = new DelegatedPermissionClassification
{
    PermissionId = "e1fe6dd8-ba31-4d61-89e7-88639da4683d",
    PermissionName = "User.Read",
    Classification = PermissionClassificationType.Low
};

await graphClient.ServicePrincipals["{servicePrincipal-id}"].DelegatedPermissionClassifications
    .Request()
    .AddAsync(delegatedPermissionClassification);

```