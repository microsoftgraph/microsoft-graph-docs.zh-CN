---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 81c26e1317a00334326f261851f7b3b23f045ce2
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61031527"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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