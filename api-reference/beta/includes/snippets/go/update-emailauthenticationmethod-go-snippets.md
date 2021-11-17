---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d4dfb71d842cc708655e1f8724591b0c51847893
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61004961"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "emailAddress": "kim@contoso.com",
}
options := &msgraphsdk.EmailAuthenticationMethodRequestBuilderPutOptions{
    Body: requestBody,
}
userId := "user-id"
emailAuthenticationMethodId := "emailAuthenticationMethod-id"
graphClient.UsersById(&userId).Authentication().EmailMethodsById(&emailAuthenticationMethodId).Put(options)


```