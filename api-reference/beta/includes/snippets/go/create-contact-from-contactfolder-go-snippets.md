---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8c7897cd7ad23790996cdcdb51db33809c766003
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328384"
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
contactFolderId := "contactFolder-id"
result, err := graphClient.Me().ContactFoldersById(&contactFolderId).Contacts().Post(requestBody)


```