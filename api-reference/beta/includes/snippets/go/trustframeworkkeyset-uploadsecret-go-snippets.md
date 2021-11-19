---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d3716caa8d94137a19dddf33e87fc08d5231f7e0
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61087799"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
use := "use-value"
requestBody.SetUse(&use)
k := "application-secret-to-be-uploaded"
requestBody.SetK(&k)
nbf := int64(1508969811)
requestBody.SetNbf(&nbf)
exp := int64(1508973711)
requestBody.SetExp(&exp)
options := &msgraphsdk.UploadSecretRequestBuilderPostOptions{
    Body: requestBody,
}
trustFrameworkKeySetId := "trustFrameworkKeySet-id"
result, err := graphClient.TrustFramework().KeySetsById(&trustFrameworkKeySetId).UploadSecret().Post(options)


```