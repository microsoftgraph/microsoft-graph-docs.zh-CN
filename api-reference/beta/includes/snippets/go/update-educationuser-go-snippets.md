---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7cf0f4c2657d701fe3f5853a509ad9a58ec7df20
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098701"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewEducationUser()
requestBody.SetRelatedContacts( []RelatedContact {
    msgraphsdk.NewRelatedContact(),
displayName := "Father Time"
    SetDisplayName(&displayName)
emailAddress := "father@time.com"
    SetEmailAddress(&emailAddress)
mobilePhone := "4251231234"
    SetMobilePhone(&mobilePhone)
relationship := "guardian"
    SetRelationship(&relationship)
accessConsent := true
    SetAccessConsent(&accessConsent)
    msgraphsdk.NewRelatedContact(),
displayName := "Mother Nature"
    SetDisplayName(&displayName)
emailAddress := "mother@nature.co.uk"
    SetEmailAddress(&emailAddress)
mobilePhone := "3251231234"
    SetMobilePhone(&mobilePhone)
relationship := "parent"
    SetRelationship(&relationship)
accessConsent := true
    SetAccessConsent(&accessConsent)
}
educationUserId := "educationUser-id"
graphClient.Education().UsersById(&educationUserId).Patch(requestBody)


```