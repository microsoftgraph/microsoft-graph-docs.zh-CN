---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 25e81c48b9f6be5271b9417698c4f0bdb7ab066f
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61007068"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

appConsentRequestId := "appConsentRequest-id"
result, err := graphClient.IdentityGovernance().AppConsent().AppConsentRequestsById(&appConsentRequestId).Get(options)


```