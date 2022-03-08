---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 957a9dbab4f55f7303703606eb42805150ca06ec
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338274"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var customAccessPackageWorkflowExtension = new CustomAccessPackageWorkflowExtension
{
    DisplayName = "test_action_0124_email",
    Description = "this is for graph testing only"
};

await graphClient.IdentityGovernance.EntitlementManagement.AccessPackageCatalogs["{accessPackageCatalog-id}"].CustomAccessPackageWorkflowExtensions["{customAccessPackageWorkflowExtension-id}"]
    .Request()
    .PutAsync(customAccessPackageWorkflowExtension);

```