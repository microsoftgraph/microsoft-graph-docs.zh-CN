---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 459fc16e7b3ee0064b5b9063e7800d5d75197711
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61008321"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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