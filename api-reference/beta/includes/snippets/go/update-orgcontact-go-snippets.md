---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f8aa2f0ce1fcc881369b257f2a6e96f240b4f3a2
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61089666"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewOrgContact()
companyName := "companyName-value"
requestBody.SetCompanyName(&companyName)
department := "department-value"
requestBody.SetDepartment(&department)
displayName := "displayName-value"
requestBody.SetDisplayName(&displayName)
requestBody.SetAdditionalData(map[string]interface{}{
    "businessPhones":  []String {
        "businessPhones-value",
    }
    "city": "city-value",
    "country": "country-value",
}
options := &msgraphsdk.OrgContactRequestBuilderPatchOptions{
    Body: requestBody,
}
orgContactId := "orgContact-id"
graphClient.ContactsById(&orgContactId).Patch(options)


```