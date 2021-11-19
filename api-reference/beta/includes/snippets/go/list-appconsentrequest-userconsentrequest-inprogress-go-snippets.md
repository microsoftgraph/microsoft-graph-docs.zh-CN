---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 348c1e7f1ce445ac62629bff241dd969731910a5
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61093557"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.AppConsentRequestsRequestBuilderGetQueryParameters{
    Filter: "userConsentRequests/any%20(u:u/status%20eq%20'InProgress')",
}
options := &msgraphsdk.AppConsentRequestsRequestBuilderGetOptions{
    Q: requestParameters,
}
result, err := graphClient.IdentityGovernance().AppConsent().AppConsentRequests().Get(options)


```