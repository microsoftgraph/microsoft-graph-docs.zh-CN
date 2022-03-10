---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 375b38e4b57c1889d76137e3087e131b9211d590
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412385"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewIdsRequestBody()
requestBody.SetIds( []String {
    "80a963dd-84af-4eb8-b2a6-781e444d4fb0",
    "62e90394-69f5-4237-9190-012177145e10",
    "86a64f51-3a64-4cc6-a8c8-6b8f000c0f52",
    "ac38546e-ddf3-437a-ac5c-27a94cd7a0f1",
}
options := &msgraphsdk.CheckMemberObjectsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Me().CheckMemberObjects().Post(options)


```