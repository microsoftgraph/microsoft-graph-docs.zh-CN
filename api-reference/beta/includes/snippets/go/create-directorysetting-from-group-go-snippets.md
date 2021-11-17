---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5d5a7adc9dfca473d64da3a3cc79508021fbb269
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61032422"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewDirectorySetting()
requestBody.SetAdditionalData(map[string]interface{}{
}
options := &msgraphsdk.SettingsRequestBuilderPostOptions{
    Body: requestBody,
}
groupId := "group-id"
result, err := graphClient.GroupsById(&groupId).Settings().Post(options)


```