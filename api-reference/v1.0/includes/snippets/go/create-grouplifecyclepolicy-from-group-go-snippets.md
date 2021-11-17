---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eb30c4111fcd79ad5fefcab0377ce86c29f9ed45
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61025267"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewGroupLifecyclePolicy()
groupLifetimeInDays := int32(100)
requestBody.SetGroupLifetimeInDays(&groupLifetimeInDays)
managedGroupTypes := "Selected"
requestBody.SetManagedGroupTypes(&managedGroupTypes)
alternateNotificationEmails := "admin@contoso.com"
requestBody.SetAlternateNotificationEmails(&alternateNotificationEmails)
options := &msgraphsdk.GroupLifecyclePoliciesRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.GroupLifecyclePolicies().Post(options)


```