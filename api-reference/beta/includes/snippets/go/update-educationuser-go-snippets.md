---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0604f463efb03aef3b50a80ccf210b33b2b9b5cb
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412420"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewEducationUser()
requestBody.SetRelatedContacts( []RelatedContact {
    msgraphsdk.NewRelatedContact(),
    SetAdditionalData(map[string]interface{}{
        "displayName": "Father Time",
        "emailAddress": "father@time.com",
        "mobilePhone": "4251231234",
        "relationship": "guardian",
        "accessConsent": true,
    }
    msgraphsdk.NewRelatedContact(),
    SetAdditionalData(map[string]interface{}{
        "displayName": "Mother Nature",
        "emailAddress": "mother@nature.co.uk",
        "mobilePhone": "3251231234",
        "relationship": "parent",
        "accessConsent": true,
    }
}
options := &msgraphsdk.EducationUserRequestBuilderPatchOptions{
    Body: requestBody,
}
educationUserId := "educationUser-id"
result, err := graphClient.Education().UsersById(&educationUserId).Patch(options)


```