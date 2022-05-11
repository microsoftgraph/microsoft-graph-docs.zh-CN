---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0d4dfa99f899b1bd1637e87b483d34b8ac423268
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326647"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAddLicenses( []AssignedLicense {
}
requestBody.SetRemoveLicenses( []String {
    "f30db892-07e9-47e9-837c-80727f46fd3d",
    "84a661c4-e949-4bd2-a560-ed7766fcaf2b",
}
result, err := graphClient.Me().AssignLicense().Post(requestBody)


```