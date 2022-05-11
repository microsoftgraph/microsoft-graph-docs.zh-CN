---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2d4a5a913e3cbb763fa82dedabb523a21c356b17
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326213"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAccessPackageResourceRoleScope()
accessPackageResourceRole := msgraphsdk.NewAccessPackageResourceRole()
requestBody.SetAccessPackageResourceRole(accessPackageResourceRole)
originId := "Member_b31fe1f1-3651-488f-bd9a-1711887fd4ca"
accessPackageResourceRole.SetOriginId(&originId)
displayName := "Member"
accessPackageResourceRole.SetDisplayName(&displayName)
originSystem := "AadGroup"
accessPackageResourceRole.SetOriginSystem(&originSystem)
accessPackageResource := msgraphsdk.NewAccessPackageResource()
accessPackageResourceRole.SetAccessPackageResource(accessPackageResource)
id := "1d08498d-72a1-403f-8511-6b1f875746a0"
accessPackageResource.SetId(&id)
resourceType := "O365 Group"
accessPackageResource.SetResourceType(&resourceType)
originId := "b31fe1f1-3651-488f-bd9a-1711887fd4ca"
accessPackageResource.SetOriginId(&originId)
originSystem := "AadGroup"
accessPackageResource.SetOriginSystem(&originSystem)
accessPackageResourceScope := msgraphsdk.NewAccessPackageResourceScope()
requestBody.SetAccessPackageResourceScope(accessPackageResourceScope)
originId := "b31fe1f1-3651-488f-bd9a-1711887fd4ca"
accessPackageResourceScope.SetOriginId(&originId)
originSystem := "AadGroup"
accessPackageResourceScope.SetOriginSystem(&originSystem)
accessPackageId := "accessPackage-id"
result, err := graphClient.IdentityGovernance().EntitlementManagement().AccessPackagesById(&accessPackageId).AccessPackageResourceRoleScopes().Post(requestBody)


```