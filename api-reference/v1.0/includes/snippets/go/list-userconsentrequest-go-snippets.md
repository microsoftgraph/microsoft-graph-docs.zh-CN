---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7ff288776f42bc4d360e8b89484d890d54af8fc6
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60992276"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

appConsentRequestId := "appConsentRequest-id"
result, err := graphClient.IdentityGovernance().AppConsent().AppConsentRequestsById(&appConsentRequestId).UserConsentRequests().Get(options)


```