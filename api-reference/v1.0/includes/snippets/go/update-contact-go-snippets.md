---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8947dcf69739e4aaa94ef308debe59e0656d86e1
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60996343"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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