---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e7ede174ff518188918ea621d7d181ef786ca656
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328129"
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
trustFrameworkKeySetId := "trustFrameworkKeySet-id"
result, err := graphClient.TrustFramework().KeySetsById(&trustFrameworkKeySetId).GenerateKey(trustFrameworkKeySet-id).Post(requestBody)


```