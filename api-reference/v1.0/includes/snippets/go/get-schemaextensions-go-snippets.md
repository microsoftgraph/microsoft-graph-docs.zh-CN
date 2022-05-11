---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 77a9acbf221b18e77243d3e692c14583e052ade4
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327773"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.SchemaExtensionsRequestBuilderGetQueryParameters{
    Filter: "id%20eq%20'graphlearn_test'",
}
options := &msgraphsdk.SchemaExtensionsRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
result, err := graphClient.SchemaExtensions().GetWithRequestConfigurationAndResponseHandler(options, nil)


```