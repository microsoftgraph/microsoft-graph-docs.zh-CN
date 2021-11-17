---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a4496d9fa1ccf4ba9cc463e0948e591e1f218421
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61013662"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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