---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 266695a90742726955d49d4bbaae92111acbf02c
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61081762"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
id := "id-value"
requestBody.SetId(&id)
groupId := "groupId-value"
requestBody.SetGroupId(&groupId)
options := &msgraphsdk.CopyToSectionRequestBuilderPostOptions{
    Body: requestBody,
}
onenotePageId := "onenotePage-id"
result, err := graphClient.Me().Onenote().PagesById(&onenotePageId).CopyToSection().Post(options)


```