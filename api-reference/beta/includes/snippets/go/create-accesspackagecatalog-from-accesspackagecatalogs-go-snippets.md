---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a746b5f37feb7e93ac14cc9e309014f0db9627fb
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60988230"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewAccessPackageCatalog()
displayName := "sales"
requestBody.SetDisplayName(&displayName)
description := "for employees working with sales and outside sales partners"
requestBody.SetDescription(&description)
isExternallyVisible := true
requestBody.SetIsExternallyVisible(&isExternallyVisible)
options := &msgraphsdk.AccessPackageCatalogsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.IdentityGovernance().EntitlementManagement().AccessPackageCatalogs().Post(options)


```