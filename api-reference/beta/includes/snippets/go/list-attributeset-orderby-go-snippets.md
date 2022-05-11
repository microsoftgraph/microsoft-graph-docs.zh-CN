---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 716e5c98d97a8c75aeb564439cb7415110bb9688
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328105"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.AttributeSetsRequestBuilderGetQueryParameters{
    OrderBy: "id",
}
options := &msgraphsdk.AttributeSetsRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
result, err := graphClient.Directory().AttributeSets().GetWithRequestConfigurationAndResponseHandler(options, nil)


```