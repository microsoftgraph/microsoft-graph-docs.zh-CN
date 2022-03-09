---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b381f96bbc97e23ccc121309d938956d1c5f28da
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63394430"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewIdentity()
id := "1431b9c38ee647f6a"
requestBody.SetId(&id)
type := "externalGroup"
requestBody.SetType(&type)
options := &msgraphsdk.MembersRequestBuilderPostOptions{
    Body: requestBody,
}
externalConnectionId := "externalConnection-id"
externalGroupId := "externalGroup-id"
result, err := graphClient.External().ConnectionsById(&externalConnectionId).GroupsById(&externalGroupId).Members().Post(options)


```