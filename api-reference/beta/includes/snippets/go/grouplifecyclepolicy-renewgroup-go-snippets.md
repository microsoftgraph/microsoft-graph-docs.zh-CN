---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 695dc1d190aac8ddcb1192a8f8b9958c99c52792
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61098696"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
groupId := "ffffffff-ffff-ffff-ffff-ffffffffffff"
requestBody.SetGroupId(&groupId)
options := &msgraphsdk.RenewGroupRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.GroupLifecyclePolicies().RenewGroup().Post(options)


```