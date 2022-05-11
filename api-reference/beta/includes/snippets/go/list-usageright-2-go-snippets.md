---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d7b22ae8136fa64bd501bae2c08e47d38b8490b2
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327923"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.UsageRightsRequestBuilderGetQueryParameters{
    Filter: "state%20in%20('active',%20'suspended')%20and%20serviceIdentifier%20in%20('ABCD')",
}
options := &msgraphsdk.UsageRightsRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
deviceId := "device-id"
result, err := graphClient.DevicesById(&deviceId).UsageRights().GetWithRequestConfigurationAndResponseHandler(options, nil)


```