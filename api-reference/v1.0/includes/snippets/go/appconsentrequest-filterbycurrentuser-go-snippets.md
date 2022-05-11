---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 041268839e098fe5b284f9b0be3f32aa39b6458d
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326539"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.AppConsentRequestRequestBuilderGetQueryParameters{
    Filter: "userConsentRequests/any(u:u/status%20eq%20'InProgress')",
}
options := &msgraphsdk.AppConsentRequestRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
appConsentRequestId := "appConsentRequest-id"
result, err := graphClient.IdentityGovernance().AppConsent().AppConsentRequestsById(&appConsentRequestId).GetWithRequestConfigurationAndResponseHandler(options, nil)


```