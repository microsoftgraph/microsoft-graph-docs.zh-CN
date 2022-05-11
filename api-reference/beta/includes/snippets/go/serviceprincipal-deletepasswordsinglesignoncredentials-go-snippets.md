---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7889caef87e9ff3992761ef2a7ba560af1174de7
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328997"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewIdRequestBody()
id := "5793aa3b-cca9-4794-679a240f8b58"
requestBody.SetId(&id)
servicePrincipalId := "servicePrincipal-id"
graphClient.ServicePrincipalsById(&servicePrincipalId).DeletePasswordSingleSignOnCredentials(servicePrincipal-id).Post(requestBody)


```