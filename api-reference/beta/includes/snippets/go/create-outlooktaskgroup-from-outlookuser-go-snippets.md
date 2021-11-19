---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 072467f5f3b6524c4ec31be0249ee91cca03910d
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61084674"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewOutlookTaskGroup()
name := "Leisure tasks"
requestBody.SetName(&name)
options := &msgraphsdk.TaskGroupsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Me().Outlook().TaskGroups().Post(options)


```