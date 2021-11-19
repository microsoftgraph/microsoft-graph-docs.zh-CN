---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9789cf9c199d7c6d947289143961eba6604475e2
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61091129"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewContact()
parentFolderId := "parentFolderId-value"
requestBody.SetParentFolderId(&parentFolderId)
birthday, err := time.Parse(time.RFC3339, "2016-10-19T10:37:00Z")
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