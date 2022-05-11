---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4e6221d5d20ff8eb90e50334c5bfe0444e79e0fc
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326211"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.id": "https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/c0a74b4d-2694-4d5d-a964-1bee4ff0aaf2",
}
accessPackageId := "accessPackage-id"
accessPackageId1 := "accessPackage-id1"
graphClient.IdentityGovernance().EntitlementManagement().AccessPackagesById(&accessPackageId).IncompatibleAccessPackagesById(&accessPackageId1).Post(requestBody)


```