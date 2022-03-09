---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e33b8048d1545cb21e0813361166eed20a919cd2
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63394423"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewIdentity()
id := "e811976d-83df-4cbd-8b9b-5215b18aa874"
requestBody.SetId(&id)
type := "user"
requestBody.SetType(&type)
options := &msgraphsdk.MembersRequestBuilderPostOptions{
    Body: requestBody,
}
externalConnectionId := "externalConnection-id"
externalGroupId := "externalGroup-id"
result, err := graphClient.External().ConnectionsById(&externalConnectionId).GroupsById(&externalGroupId).Members().Post(options)


```