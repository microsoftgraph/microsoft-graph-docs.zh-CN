---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eec126c6c81d93530037859fffa437c6d6165134
ms.sourcegitcommit: 1d9193fa91f44d80ecdc2b82e37272df1c9630f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/22/2022
ms.locfileid: "65629800"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.SitesRequestBuilderGetQueryParameters{
    Search: "%7Bquery%7D",
}
options := &msgraphsdk.SitesRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
result, err := graphClient.Sites().GetWithRequestConfigurationAndResponseHandler(options, nil)


```