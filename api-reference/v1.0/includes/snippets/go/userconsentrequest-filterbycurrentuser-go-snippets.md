---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 574b2b8f5fa685774bd26262c6bfc69331ec41cf
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61086683"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.UserConsentRequestRequestBuilderGetQueryParameters{
    Filter: "%20(status%20eq%20'Completed')",
}
options := &msgraphsdk.UserConsentRequestRequestBuilderGetOptions{
    Q: requestParameters,
}
appConsentRequestId := "appConsentRequest-id"
userConsentRequestId := "userConsentRequest-id"
result, err := graphClient.IdentityGovernance().AppConsent().AppConsentRequestsById(&appConsentRequestId).UserConsentRequestsById(&userConsentRequestId).Get(options)


```