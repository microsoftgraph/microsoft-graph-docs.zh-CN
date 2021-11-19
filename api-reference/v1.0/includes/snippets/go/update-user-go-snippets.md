---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bf3777b4940826dd96715ab78ee421fa61d6e223
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61081750"
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
options := &msgraphsdk.MeRequestBuilderPatchOptions{
    Body: requestBody,
}
graphClient.Me().Patch(options)


```