---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 14077e7fd0ebddd3ec06a35344c103ee5916509a
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60985849"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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