---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 36f71a5f961ae7c0a443f9b44eaf20af0be74d30
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61085988"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.B2xUserFlowsRequestBuilderGetQueryParameters{
    Expand: "identityProviders",
}
options := &msgraphsdk.B2xUserFlowsRequestBuilderGetOptions{
    Q: requestParameters,
}
result, err := graphClient.Identity().B2xUserFlows().Get(options)


```