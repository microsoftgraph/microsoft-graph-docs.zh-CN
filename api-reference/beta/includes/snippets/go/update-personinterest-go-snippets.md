---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1d871c2d327cfba4c29e9d6f5dc2bdef7c63140d
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61103928"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewPersonInterest()
requestBody.SetCategories( []String {
    "Sports",
}
options := &msgraphsdk.PersonInterestRequestBuilderPatchOptions{
    Body: requestBody,
}
personInterestId := "personInterest-id"
graphClient.Me().Profile().InterestsById(&personInterestId).Patch(options)


```