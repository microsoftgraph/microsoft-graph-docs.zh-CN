---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aa885f35910951ea7ff33bb508c003cd5748e53c
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61020143"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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