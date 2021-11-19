---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a2df90d9f110b7d8a76cb05ebd84a9ca0f525975
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61092520"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.B2cUserFlowsRequestBuilderGetQueryParameters{
    Expand: "identityProviders",
}
options := &msgraphsdk.B2cUserFlowsRequestBuilderGetOptions{
    Q: requestParameters,
}
result, err := graphClient.Identity().B2cUserFlows().Get(options)


```