---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dd7a5faca41b8eeed5752545ca07ccb6bcf3db66
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328683"
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
directoryObjectId := "directoryObject-id"
result, err := graphClient.DirectoryObjectsById(&directoryObjectId).CheckMemberGroups(directoryObject-id).Post(requestBody)


```