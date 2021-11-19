---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4575e398de2acbd5bb70a60be42fc4338e3beec7
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61097974"
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
graphClient.Me().Outlook().TaskFoldersById(&outlookTaskFolderId).Patch(options)


```