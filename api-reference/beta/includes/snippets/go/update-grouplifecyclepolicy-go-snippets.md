---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8891472d0011d198dc10e0800c62e6302022d210
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411659"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewGroupLifecyclePolicy()
groupLifetimeInDays := int32(180)
requestBody.SetGroupLifetimeInDays(&groupLifetimeInDays)
managedGroupTypes := "Selected"
requestBody.SetManagedGroupTypes(&managedGroupTypes)
alternateNotificationEmails := "admin@contoso.com"
requestBody.SetAlternateNotificationEmails(&alternateNotificationEmails)
options := &msgraphsdk.GroupLifecyclePolicyRequestBuilderPatchOptions{
    Body: requestBody,
}
groupLifecyclePolicyId := "groupLifecyclePolicy-id"
result, err := graphClient.GroupLifecyclePoliciesById(&groupLifecyclePolicyId).Patch(options)


```