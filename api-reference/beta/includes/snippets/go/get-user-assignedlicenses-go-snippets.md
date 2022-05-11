---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c4ab702dd31625d6f09c50831757cd6018ce8d11
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327945"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.UsersRequestBuilderGetQueryParameters{
    Select: "id,mail,assignedLicenses",
    Filter: "assignedLicenses/any(u:u/skuId%20eq%20cbdc14ab-d96c-4c30-b9f4-6ada7cdc1d46)",
}
options := &msgraphsdk.UsersRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
result, err := graphClient.Users().GetWithRequestConfigurationAndResponseHandler(options, nil)


```