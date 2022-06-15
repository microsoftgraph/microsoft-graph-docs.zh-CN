---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fec6aaee2044680cf7ca80a41130c59fee4a6526
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098823"
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
number := "+1 732 555 0102"
    SetNumber(&number)
type := "business"
    SetType(&type)
}
result, err := graphClient.Me().Contacts().Post(requestBody)


```