---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2dae3578c01a3da7bfa05f6ee7ee3af7c306e2fd
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098707"
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
address := "pavelb@fabrikam.onmicrosoft.com"
    SetAddress(&address)
name := "Pavel Bansky"
    SetName(&name)
}
requestBody.SetBusinessPhones( []String {
    "+1 732 555 0102",
}
result, err := graphClient.Me().Contacts().Post(requestBody)


```