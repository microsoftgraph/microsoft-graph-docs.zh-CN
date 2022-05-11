---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c628d12d9be1e52f9a6ba50ba5676b8c29319c9e
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328299"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.DirectoryObjectRequestBuilderGetQueryParameters{
    Count: true,
    OrderBy: "displayName",
    Filter: "startswith(displayName,%20'A')",
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
result, err := graphClient.DevicesById(&deviceId).MemberOfById(&directoryObjectId).GetWithRequestConfigurationAndResponseHandler(options, nil)


```