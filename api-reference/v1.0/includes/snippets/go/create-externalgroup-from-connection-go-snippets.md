---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 08afe4c472f21fc48769376686f9acb096c89ccf
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63393239"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewExternalGroup()
id := "31bea3d537902000"
requestBody.SetId(&id)
displayName := "Contoso Marketing"
requestBody.SetDisplayName(&displayName)
description := "The product marketing team"
requestBody.SetDescription(&description)
options := &msgraphsdk.GroupsRequestBuilderPostOptions{
    Body: requestBody,
}
externalConnectionId := "externalConnection-id"
result, err := graphClient.External().ConnectionsById(&externalConnectionId).Groups().Post(options)


```