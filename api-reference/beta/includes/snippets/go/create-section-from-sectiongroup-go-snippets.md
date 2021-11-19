---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9316fad766a8b1a76ee8f0bb4235ecf602fc7274
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61085774"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewOnenoteSection()
displayName := "Section name"
requestBody.SetDisplayName(&displayName)
options := &msgraphsdk.SectionsRequestBuilderPostOptions{
    Body: requestBody,
}
sectionGroupId := "sectionGroup-id"
result, err := graphClient.Me().Onenote().SectionGroupsById(&sectionGroupId).Sections().Post(options)


```