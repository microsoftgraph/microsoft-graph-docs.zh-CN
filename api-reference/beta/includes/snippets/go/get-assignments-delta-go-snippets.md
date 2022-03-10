---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1189ab44b517b3da8d06d83450a3902b311b8ee6
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412299"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.DeltaRequestBuilderGetQueryParameters{
    Deltatoken: "7ORzTfzlUEGDy6BRE3OC-3ePBbvLHCRe4aJ_hjaBKJxUHmn_ODgoM4xreLS7YRaxROmLjac48n-iXm5j6n5aQwlsnC-2OvL3lI0Z8M4klERNmJQjnBn7MHqwXZ6L8GlI3VPnya3E-p1bisiZX97jLvQUAopseIYhvnD6v7fiYrk.fVsHempT6X2CiBh6aN9Ex5nVJ71adKdcf-mdke8OHKs",
}
options := &msgraphsdk.DeltaRequestBuilderGetOptions{
    Q: requestParameters,
}
educationClassId := "educationClass-id"
result, err := graphClient.Education().ClassesById(&educationClassId).Assignments().Delta()(educationClass-id).Get(options)


```