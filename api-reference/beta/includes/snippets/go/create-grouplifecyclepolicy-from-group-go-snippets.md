---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0fd6335b7e0059912c5bef00704059150213207d
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61088536"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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