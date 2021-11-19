---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 44bf396231e6a92ceccef47d58eab4f77694772a
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61103122"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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