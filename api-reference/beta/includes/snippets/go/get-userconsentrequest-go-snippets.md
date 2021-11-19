---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 338dbb1271ed16e2bd42f950337c6993e609c8d8
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61092049"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

appConsentRequestId := "appConsentRequest-id"
userConsentRequestId := "userConsentRequest-id"
result, err := graphClient.IdentityGovernance().AppConsent().AppConsentRequestsById(&appConsentRequestId).UserConsentRequestsById(&userConsentRequestId).Get(options)


```