---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2fd42f97597bcd314a4f9fbf5b73f27f4f54d9e2
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60997673"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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