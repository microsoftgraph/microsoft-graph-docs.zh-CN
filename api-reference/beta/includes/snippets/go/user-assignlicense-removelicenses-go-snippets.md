---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e3bbba6ed212998a92fca53cb5c2872a0a468831
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63339971"
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
options := &msgraphsdk.AssignLicenseRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Me().AssignLicense().Post(options)


```