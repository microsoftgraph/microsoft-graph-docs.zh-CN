---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5855e84d1ccc5ff79827ca4eb7f8e1b7e4884860
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61084778"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
use := "sig"
requestBody.SetUse(&use)
kty := "RSA"
requestBody.SetKty(&kty)
nbf := int64(1508969811)
requestBody.SetNbf(&nbf)
exp := int64(1508969811)
requestBody.SetExp(&exp)
options := &msgraphsdk.GenerateKeyRequestBuilderPostOptions{
    Body: requestBody,
}
trustFrameworkKeySetId := "trustFrameworkKeySet-id"
result, err := graphClient.TrustFramework().KeySetsById(&trustFrameworkKeySetId).GenerateKey().Post(options)


```