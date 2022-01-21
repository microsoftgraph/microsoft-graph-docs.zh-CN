---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1691626699ac4b40e4870f96d56208f341f78639
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62137742"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.DeltaRequestBuilderGetQueryParameters{
    Deltatoken: "7ORzTfzlUEGDy6BRE3OC-3ePBbvLHCRe4aJ_hjaBKJxUHmn_ODgoM4xreLS7YRaxc-iACeqCQsT5Tb0u9vn6QXYflO6j0sRgRQlhcfR7DApZYl6uZqiXcR7H0G14btPqR761sKWNc0jgiczrHGF6dGfSQwsLzPT46og-84ArhOU.Jnxvkr08FE-QBvEYstYel3JZUrgwgTauo-GmpbdWeSA",
}
options := &msgraphsdk.DeltaRequestBuilderGetOptions{
    Q: requestParameters,
}
educationClassId := "educationClass-id"
result, err := graphClient.Education().ClassesById(&educationClassId).AssignmentCategories().Delta()().Get(options)


```