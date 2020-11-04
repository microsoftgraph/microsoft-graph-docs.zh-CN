---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fe0d529fe790ef41c4f6cb99d25c28ec6ef00c7c
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48904780"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delegatedPermissionClassification = new DelegatedPermissionClassification
{
    PermissionId = "e1fe6dd8-ba31-4d61-89e7-88639da4683d",
    PermissionName = "User.Read",
    Classification = PermissionClassificationType.Low
};

await graphClient.ServicePrincipals["{id}"].DelegatedPermissionClassifications
    .Request()
    .AddAsync(delegatedPermissionClassification);

```