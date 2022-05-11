---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1cd18208429eff0c2de7d9d4fb247d9bf625f55b
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328007"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.LanguagesRequestBuilderGetQueryParameters{
    Filter: "isEnabled%20eq%20true",
}
options := &msgraphsdk.LanguagesRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
b2cIdentityUserFlowId := "b2cIdentityUserFlow-id"
result, err := graphClient.Identity().B2cUserFlowsById(&b2cIdentityUserFlowId).Languages().GetWithRequestConfigurationAndResponseHandler(options, nil)


```