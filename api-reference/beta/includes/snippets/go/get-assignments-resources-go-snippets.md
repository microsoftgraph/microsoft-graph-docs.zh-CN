---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e791bae199529bb1187027bcd13e59b76cc267d9
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325870"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.AssignmentsRequestBuilderGetQueryParameters{
    Expand: "resources",
}
options := &msgraphsdk.AssignmentsRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
educationClassId := "educationClass-id"
result, err := graphClient.Education().ClassesById(&educationClassId).Assignments().GetWithRequestConfigurationAndResponseHandler(options, nil)


```