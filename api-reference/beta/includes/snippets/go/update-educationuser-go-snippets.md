---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 742a22e8f32fec8a28322019850fced0bd529ce7
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/08/2022
ms.locfileid: "65946827"
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
educationUserId := "educationUser-id"
graphClient.Education().UsersById(&educationUserId).Patch(requestBody)


```