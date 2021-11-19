---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4264f373994fb53a3291351a0c98c9c141e76b0f
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61085073"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewContact()
homeAddress := msgraphsdk.NewPhysicalAddress()
requestBody.SetHomeAddress(homeAddress)
street := "123 Some street"
homeAddress.SetStreet(&street)
city := "Seattle"
homeAddress.SetCity(&city)
state := "WA"
homeAddress.SetState(&state)
postalCode := "98121"
homeAddress.SetPostalCode(&postalCode)
birthday, err := time.Parse(time.RFC3339, "1974-07-22")
requestBody.SetBirthday(&birthday)
options := &msgraphsdk.ContactRequestBuilderPatchOptions{
    Body: requestBody,
}
contactId := "contact-id"
graphClient.Me().ContactsById(&contactId).Patch(options)


```