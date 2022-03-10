---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 489f28432a3fc4e057cef67756a47157e4c6c524
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412334"
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
result, err := graphClient.Me().ContactsById(&contactId).Patch(options)


```