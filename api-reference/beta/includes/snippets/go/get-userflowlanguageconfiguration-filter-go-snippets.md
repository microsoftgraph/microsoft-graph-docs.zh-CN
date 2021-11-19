---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 29df077206bfed303490ef9e2f196ce71231390a
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61093722"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.LanguagesRequestBuilderGetQueryParameters{
    Filter: "isEnabled%20eq%20true",
}
options := &msgraphsdk.LanguagesRequestBuilderGetOptions{
    Q: requestParameters,
}
b2cIdentityUserFlowId := "b2cIdentityUserFlow-id"
result, err := graphClient.Identity().B2cUserFlowsById(&b2cIdentityUserFlowId).Languages().Get(options)


```