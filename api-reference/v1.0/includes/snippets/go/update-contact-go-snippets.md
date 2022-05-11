---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cc46307c6da6f9ab4ca53605e7140ebf1e329347
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327081"
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
contactId := "contact-id"
graphClient.Me().ContactsById(&contactId).Patch(requestBody)


```