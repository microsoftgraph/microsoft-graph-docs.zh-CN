---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b8feb9506c16c7fb51b0e9a97943e3323ec0d761
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2021
ms.locfileid: "61348778"
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
graphClient.Education().UsersById(&educationUserId).Patch(options)


```