---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a6a84cb8e063b907f855dbe91b9726b931677282
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60986111"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.B2cUserFlowsRequestBuilderGetQueryParameters{
    Expand: "identityProviders",
}
options := &msgraphsdk.B2cUserFlowsRequestBuilderGetOptions{
    Q: requestParameters,
}
result, err := graphClient.Identity().B2cUserFlows().Get(options)


```