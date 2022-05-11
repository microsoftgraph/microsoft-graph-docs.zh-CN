---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ee965ac2b4fbf189bc38e8c785fc39da06d752e3
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328121"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.UserConsentRequestRequestBuilderGetQueryParameters{
    Filter: "%20(status%20eq%20'Completed')",
}
options := &msgraphsdk.UserConsentRequestRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
appConsentRequestId := "appConsentRequest-id"
userConsentRequestId := "userConsentRequest-id"
result, err := graphClient.IdentityGovernance().AppConsent().AppConsentRequestsById(&appConsentRequestId).UserConsentRequestsById(&userConsentRequestId).GetWithRequestConfigurationAndResponseHandler(options, nil)


```