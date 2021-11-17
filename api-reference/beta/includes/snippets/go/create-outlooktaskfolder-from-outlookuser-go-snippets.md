---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 27cace219dddd3870f78a3e0d9a967d44cb4b3a6
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61026555"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewOutlookTaskFolder()
name := "Volunteer"
requestBody.SetName(&name)
options := &msgraphsdk.TaskFoldersRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Me().Outlook().TaskFolders().Post(options)


```