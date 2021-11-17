---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d116664d5606b2b78d483435292632be2e39271f
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61031372"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewContact()
givenName := "Pavel"
requestBody.SetGivenName(&givenName)
surname := "Bansky"
requestBody.SetSurname(&surname)
requestBody.SetEmailAddresses( []TypedEmailAddress {
    msgraphsdk.NewTypedEmailAddress(),
    SetAdditionalData(map[string]interface{}{
        "address": "pavelb@contoso.onmicrosoft.com",
        "name": "Pavel Bansky",
        "type": "personal",
    }
    msgraphsdk.NewTypedEmailAddress(),
    SetAdditionalData(map[string]interface{}{
        "address": "pavelb@fabrikam.onmicrosoft.com",
        "name": "Pavel Bansky",
        "type": "other",
        "otherLabel": "Volunteer work",
    }
}
requestBody.SetPhones( []Phone {
    msgraphsdk.NewPhone(),
    SetAdditionalData(map[string]interface{}{
        "number": "+1 732 555 0102",
        "type": "business",
    }
}
options := &msgraphsdk.ContactsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Me().Contacts().Post(options)


```