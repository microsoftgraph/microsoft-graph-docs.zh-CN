---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 194745516d834802bf16bddb5b61e2e9310a994a
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326635"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.DirectoryObjectRequestBuilderGetQueryParameters{
    Count: true,
    OrderBy: "displayName",
    Filter: "startswith(displayName,%20'a')",
}
headers := map[string]string{
    "ConsistencyLevel": "eventual"
}
options := &msgraphsdk.DirectoryObjectRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
    Headers: headers,
}
deviceId := "device-id"
directoryObjectId := "directoryObject-id"
result, err := graphClient.DevicesById(&deviceId).TransitiveMemberOfById(&directoryObjectId).GetWithRequestConfigurationAndResponseHandler(options, nil)


```