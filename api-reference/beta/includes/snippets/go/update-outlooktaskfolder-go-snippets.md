---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 05a0a0c5769ac616214bea8450be1c5a26aa1923
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412241"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewOutlookTaskFolder()
name := "Charity work"
requestBody.SetName(&name)
options := &msgraphsdk.OutlookTaskFolderRequestBuilderPatchOptions{
    Body: requestBody,
}
outlookTaskFolderId := "outlookTaskFolder-id"
result, err := graphClient.Me().Outlook().TaskFoldersById(&outlookTaskFolderId).Patch(options)


```