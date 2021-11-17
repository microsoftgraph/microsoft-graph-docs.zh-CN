---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f5867aa2b9b8759eea7f597db5c2ed089f87db8d
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60998199"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.B2xUserFlowsRequestBuilderGetQueryParameters{
    Expand: "identityProviders",
}
options := &msgraphsdk.B2xUserFlowsRequestBuilderGetOptions{
    Q: requestParameters,
}
result, err := graphClient.Identity().B2xUserFlows().Get(options)


```