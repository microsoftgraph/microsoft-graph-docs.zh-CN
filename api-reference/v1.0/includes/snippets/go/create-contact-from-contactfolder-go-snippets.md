---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0a563ddf6f4db9bf6048d69caa806d40ad0ce5f1
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60974311"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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