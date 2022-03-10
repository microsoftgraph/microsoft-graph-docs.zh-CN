---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4fc2f2d82524b836a6a2c18f8a5feda30d0e9502
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412656"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewGroupIdsRequestBody()
requestBody.SetGroupIds( []String {
    "f448435d-3ca7-4073-8152-a1fd73c0fd09",
    "bd7c6263-4dd5-4ae8-8c96-556e1c0bece6",
    "93670da6-d731-4366-94b5-abed40b6016b",
    "f5484ab1-4d4d-41ec-a9b8-754b3957bfc7",
    "c9103f26-f3cf-4004-a611-2a14e81b8f79",
}
options := &msgraphsdk.CheckMemberGroupsRequestBuilderPostOptions{
    Body: requestBody,
}
directoryObjectId := "directoryObject-id"
result, err := graphClient.DirectoryObjectsById(&directoryObjectId).CheckMemberGroups(directoryObject-id).Post(options)


```