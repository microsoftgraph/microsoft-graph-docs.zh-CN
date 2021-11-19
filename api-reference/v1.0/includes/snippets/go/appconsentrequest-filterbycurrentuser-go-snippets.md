---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 86a31fc5b1846eb1694546efc89d9950031daaca
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61100351"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.AppConsentRequestRequestBuilderGetQueryParameters{
    Filter: "userConsentRequests/any(u:u/status%20eq%20'InProgress')",
}
options := &msgraphsdk.AppConsentRequestRequestBuilderGetOptions{
    Q: requestParameters,
}
appConsentRequestId := "appConsentRequest-id"
result, err := graphClient.IdentityGovernance().AppConsent().AppConsentRequestsById(&appConsentRequestId).Get(options)


```