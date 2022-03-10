---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6e0ee96cd36b3b21bf4ce3bbc4f6b6e6aca1fa0d
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411701"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.id": "https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/c0a74b4d-2694-4d5d-a964-1bee4ff0aaf2",
}
options := &msgraphsdk.AccessPackageRequestBuilderPostOptions{
    Body: requestBody,
}
accessPackageId := "accessPackage-id"
accessPackageId1 := "accessPackage-id1"
graphClient.IdentityGovernance().EntitlementManagement().AccessPackagesById(&accessPackageId).IncompatibleAccessPackagesById(&accessPackageId1).Post(options)


```