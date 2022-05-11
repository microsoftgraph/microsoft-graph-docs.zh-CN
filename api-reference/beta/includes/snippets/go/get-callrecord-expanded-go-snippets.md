---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 885b3d50b03721c3d1f0dc4fcca3e3a0ffd2edd1
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327030"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.CallRecordRequestBuilderGetQueryParameters{
    Expand: "sessions($expand=segments)",
}
options := &msgraphsdk.CallRecordRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
callRecordId := "callRecord-id"
result, err := graphClient.Communications().CallRecordsById(&callRecordId).GetWithRequestConfigurationAndResponseHandler(options, nil)


```