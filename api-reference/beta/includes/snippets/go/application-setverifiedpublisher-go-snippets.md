---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 529dc0345b9247ca116bb706743c95c39e7f1e19
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60982854"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.New()
verifiedPublisherId := "1234567"
requestBody.SetVerifiedPublisherId(&verifiedPublisherId)
options := &msgraphsdk.SetVerifiedPublisherRequestBuilderPostOptions{
    Body: requestBody,
}
applicationId := "application-id"
graphClient.ApplicationsById(&applicationId).SetVerifiedPublisher().Post(options)


```