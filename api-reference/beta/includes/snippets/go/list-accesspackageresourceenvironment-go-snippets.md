---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bbe242ab2e4c2beace2a96996e55d67e8aa4eda2
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61087554"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.AccessPackageResourceEnvironmentsRequestBuilderGetQueryParameters{
    Filter: "originSystem%20eq%20'SharePointOnline'",
}
options := &msgraphsdk.AccessPackageResourceEnvironmentsRequestBuilderGetOptions{
    Q: requestParameters,
}
result, err := graphClient.IdentityGovernance().EntitlementManagement().AccessPackageResourceEnvironments().Get(options)


```