---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3be0da11bbdcff464ea178c2ff8bf16551203d05
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61082161"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
id := "id-value"
requestBody.SetId(&id)
groupId := "groupId-value"
requestBody.SetGroupId(&groupId)
renameAs := "renameAs-value"
requestBody.SetRenameAs(&renameAs)
options := &msgraphsdk.CopyToSectionGroupRequestBuilderPostOptions{
    Body: requestBody,
}
onenoteSectionId := "onenoteSection-id"
result, err := graphClient.Me().Onenote().SectionsById(&onenoteSectionId).CopyToSectionGroup().Post(options)


```