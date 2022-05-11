---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 83f90ca06ffb5807b9811d73492b07fbff34daf1
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327725"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.EventsRequestBuilderGetQueryParameters{
    Filter: "startsWith(subject,'All')",
}
options := &msgraphsdk.EventsRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
result, err := graphClient.Me().Calendar().Events().GetWithRequestConfigurationAndResponseHandler(options, nil)


```