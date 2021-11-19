---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e960e5afde70867c1a3ee1dcdb0dd823a6c79cad
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61082803"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewContact()
parentFolderId := "parentFolderId-value"
requestBody.SetParentFolderId(&parentFolderId)
birthday, err := time.Parse(time.RFC3339, "datetime-value")
requestBody.SetBirthday(&birthday)
fileAs := "fileAs-value"
requestBody.SetFileAs(&fileAs)
displayName := "displayName-value"
requestBody.SetDisplayName(&displayName)
givenName := "givenName-value"
requestBody.SetGivenName(&givenName)
initials := "initials-value"
requestBody.SetInitials(&initials)
options := &msgraphsdk.ContactsRequestBuilderPostOptions{
    Body: requestBody,
}
contactFolderId := "contactFolder-id"
result, err := graphClient.Me().ContactFoldersById(&contactFolderId).Contacts().Post(options)


```