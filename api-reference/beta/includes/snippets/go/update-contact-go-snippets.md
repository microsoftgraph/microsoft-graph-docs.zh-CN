---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c2e2008e7eb1ce190737c1cb42e98c5908d19c58
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60990287"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewContact()
requestBody.SetEmailAddresses( []TypedEmailAddress {
    msgraphsdk.NewTypedEmailAddress(),
    SetAdditionalData(map[string]interface{}{
        "type": "personal",
        "name": "Pavel Bansky",
        "address": "pavelb@adatum.onmicrosoft.com",
    }
    msgraphsdk.NewTypedEmailAddress(),
    SetAdditionalData(map[string]interface{}{
        "address": "pavelb@fabrikam.onmicrosoft.com",
        "name": "Pavel Bansky",
        "type": "other",
        "otherLabel": "Volunteer work",
    }
}
options := &msgraphsdk.ContactRequestBuilderPatchOptions{
    Body: requestBody,
}
contactId := "contact-id"
graphClient.Me().ContactsById(&contactId).Patch(options)


```