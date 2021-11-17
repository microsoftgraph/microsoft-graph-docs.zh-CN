---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0e6e67fff9cb90baa3edf60b4ebe785d4354a56c
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61026646"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewEducationClass()
description := "Health Level 1"
requestBody.SetDescription(&description)
classCode := "Health 501"
requestBody.SetClassCode(&classCode)
displayName := "Health 1"
requestBody.SetDisplayName(&displayName)
externalId := "11019"
requestBody.SetExternalId(&externalId)
externalName := "Health Level 1"
requestBody.SetExternalName(&externalName)
externalSource := "sis"
requestBody.SetExternalSource(&externalSource)
mailNickname := "fineartschool.net"
requestBody.SetMailNickname(&mailNickname)
options := &msgraphsdk.ClassesRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Education().Classes().Post(options)


```