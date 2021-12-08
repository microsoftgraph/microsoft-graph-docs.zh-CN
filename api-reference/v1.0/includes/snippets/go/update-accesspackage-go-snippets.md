---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 98fae05166422e52044419de3701677a4306cbb8
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2021
ms.locfileid: "61334948"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAccessPackage()
displayName := "Access Package New Name"
requestBody.SetDisplayName(&displayName)
options := &msgraphsdk.AccessPackageRequestBuilderPatchOptions{
    Body: requestBody,
}
accessPackageId := "accessPackage-id"
graphClient.IdentityGovernance().EntitlementManagement().AccessPackagesById(&accessPackageId).Patch(options)


```