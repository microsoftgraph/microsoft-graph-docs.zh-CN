---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ac0443f29997e7be0b34ff2e7ad7c32944336f63
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60999937"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.LanguagesRequestBuilderGetQueryParameters{
    Filter: "isEnabled%20eq%20true",
}
options := &msgraphsdk.LanguagesRequestBuilderGetOptions{
    Q: requestParameters,
}
b2cIdentityUserFlowId := "b2cIdentityUserFlow-id"
result, err := graphClient.Identity().B2cUserFlowsById(&b2cIdentityUserFlowId).Languages().Get(options)


```