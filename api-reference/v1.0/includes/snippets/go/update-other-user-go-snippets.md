---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 56702dd4cfed73fa2ebe0e7e2909058fda77eac4
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412429"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewUser()
requestBody.SetBusinessPhones( []String {
    "+1 425 555 0109",
}
officeLocation := "18/2111"
requestBody.SetOfficeLocation(&officeLocation)
options := &msgraphsdk.UserRequestBuilderPatchOptions{
    Body: requestBody,
}
userId := "user-id"
result, err := graphClient.UsersById(&userId).Patch(options)


```