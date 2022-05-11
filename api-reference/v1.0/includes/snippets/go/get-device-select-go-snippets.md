---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 866217518b712c216c8837a04a4c428d9dcef9d3
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326744"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.DeviceRequestBuilderGetQueryParameters{
    Select: "id,extensionAttributes",
}
options := &msgraphsdk.DeviceRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
deviceId := "device-id"
result, err := graphClient.DevicesById(&deviceId).GetWithRequestConfigurationAndResponseHandler(options, nil)


```