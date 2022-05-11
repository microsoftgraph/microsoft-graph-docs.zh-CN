---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: be5fcce952c91e65a4b33673105c1e2b741ad8d1
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327878"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
key := "Base64-encoded-pfx-content"
requestBody.SetKey(&key)
password := "password-value"
requestBody.SetPassword(&password)
trustFrameworkKeySetId := "trustFrameworkKeySet-id"
result, err := graphClient.TrustFramework().KeySetsById(&trustFrameworkKeySetId).UploadPkcs12(trustFrameworkKeySet-id).Post(requestBody)


```