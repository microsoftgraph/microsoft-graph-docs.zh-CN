---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 212bf33118b7d3352efa628dfee3466fe42bab78
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61082253"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewContact()
givenName := "Pavel"
requestBody.SetGivenName(&givenName)
surname := "Bansky"
requestBody.SetSurname(&surname)
requestBody.SetEmailAddresses( []EmailAddress {
    msgraphsdk.NewEmailAddress(),
    SetAdditionalData(map[string]interface{}{
        "address": "pavelb@fabrikam.onmicrosoft.com",
        "name": "Pavel Bansky",
    }
}
requestBody.SetBusinessPhones( []String {
    "+1 732 555 0102",
}
options := &msgraphsdk.ContactsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Me().Contacts().Post(options)


```