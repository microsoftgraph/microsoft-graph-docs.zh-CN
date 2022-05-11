---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f451a658fcff9d714c7d32960c336dadfe10c044
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326104"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.AppConsentRequestsRequestBuilderGetQueryParameters{
    Filter: "userConsentRequests/any%20(u:u/status%20eq%20'InProgress')",
}
options := &msgraphsdk.AppConsentRequestsRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
result, err := graphClient.IdentityGovernance().AppConsent().AppConsentRequests().GetWithRequestConfigurationAndResponseHandler(options, nil)


```