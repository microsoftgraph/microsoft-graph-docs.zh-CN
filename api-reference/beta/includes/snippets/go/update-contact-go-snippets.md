---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 927f5448b30a8846492d50829efd179aa9338060
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412055"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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
result, err := graphClient.Me().ContactsById(&contactId).Patch(options)


```