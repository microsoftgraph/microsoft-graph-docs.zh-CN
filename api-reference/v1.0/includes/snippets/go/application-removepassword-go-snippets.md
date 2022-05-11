---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5a9616a2fe3ddc81e9a3ad1017abb1c3a69c0539
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326976"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewKeyIdRequestBody()
keyId := "f0b0b335-1d71-4883-8f98-567911bfdca6"
requestBody.SetKeyId(&keyId)
applicationId := "application-id"
graphClient.ApplicationsById(&applicationId).RemovePassword(application-id).Post(requestBody)


```