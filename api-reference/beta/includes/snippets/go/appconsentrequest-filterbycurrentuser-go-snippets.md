---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f5865f27928edc32223f98337040bfa278699398
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60995622"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.AppConsentRequestRequestBuilderGetQueryParameters{
    Filter: "userConsentRequests/any(u:u/status%20eq%20'InProgress')",
}
options := &msgraphsdk.AppConsentRequestRequestBuilderGetOptions{
    Q: requestParameters,
}
appConsentRequestId := "appConsentRequest-id"
result, err := graphClient.IdentityGovernance().AppConsent().AppConsentRequestsById(&appConsentRequestId).Get(options)


```