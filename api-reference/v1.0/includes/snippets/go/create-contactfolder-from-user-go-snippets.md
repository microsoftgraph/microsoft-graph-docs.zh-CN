---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7bd99ec4a251b7e65c6bd7dfa2b50cf88d21d241
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61020157"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewContactFolder()
parentFolderId := "AQMkADIxYjJiYgEzLTFmNjYALTRjYTMtODA1NC0wZDkxZGNmOTcxNTQALgAAA8RJzXYaLKZPlmn0ge0edZkBADa3qi2IMXRNg6RwQSHe_F8AAAIBDgAAAA=="
requestBody.SetParentFolderId(&parentFolderId)
displayName := "Important contacts"
requestBody.SetDisplayName(&displayName)
options := &msgraphsdk.ContactFoldersRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Me().ContactFolders().Post(options)


```