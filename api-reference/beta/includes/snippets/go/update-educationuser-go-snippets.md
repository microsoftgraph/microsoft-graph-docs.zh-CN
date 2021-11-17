---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 732bbebb5e303af36bc60bc3136e7c646355d574
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61005051"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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