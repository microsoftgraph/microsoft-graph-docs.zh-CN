---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7a8d5fb3379f8d3d0c991055f76ea5b9cb7290fc
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61018421"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
}
options := &msgraphsdk.MemberOfRequestBuilderPostOptions{
    Body: requestBody,
}
orgContactId := "orgContact-id"
graphClient.ContactsById(&orgContactId).MemberOf().Post(options)


```