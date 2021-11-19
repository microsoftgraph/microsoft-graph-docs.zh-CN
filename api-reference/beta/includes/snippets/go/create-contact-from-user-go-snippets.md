---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 039f656b0efac60d3fd4fae220e20ffc261917a7
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61091774"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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