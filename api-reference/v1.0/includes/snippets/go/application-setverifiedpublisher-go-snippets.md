---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1eb3eee4f9a1d3259b10fd694881857febb07ad1
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327597"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewVerifiedPublisherIdRequestBody()
verifiedPublisherId := "1234567"
requestBody.SetVerifiedPublisherId(&verifiedPublisherId)
applicationId := "application-id"
graphClient.ApplicationsById(&applicationId).SetVerifiedPublisher(application-id).Post(requestBody)


```