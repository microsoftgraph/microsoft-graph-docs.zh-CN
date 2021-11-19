---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5bbd614ec3a8a3558010f1a5d99faa6c9bbfed6e
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61102303"
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
graphClient.Me().ContactsById(&contactId).Patch(options)


```