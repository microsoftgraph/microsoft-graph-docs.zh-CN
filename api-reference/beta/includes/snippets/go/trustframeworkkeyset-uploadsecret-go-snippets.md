---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1ca50980303a8028c5668f780d2264dd51654990
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411944"
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
result, err := graphClient.TrustFramework().KeySetsById(&trustFrameworkKeySetId).UploadSecret(trustFrameworkKeySet-id).Post(options)


```