---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4dbd98027124979ff7b3eba1131f0033510fcfb4
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326098"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewPasswordCredentialRequestBody()
passwordCredential := msgraphsdk.NewPasswordCredential()
requestBody.SetPasswordCredential(passwordCredential)
displayName := "Password friendly name"
passwordCredential.SetDisplayName(&displayName)
applicationId := "application-id"
result, err := graphClient.ApplicationsById(&applicationId).AddPassword(application-id).Post(requestBody)


```