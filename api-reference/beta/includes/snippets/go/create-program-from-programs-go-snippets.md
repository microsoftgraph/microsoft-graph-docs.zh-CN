---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a39dba22c881bf0f75aa4c03ffb78443f049773c
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61091715"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewProgram()
displayName := "testprogram3"
requestBody.SetDisplayName(&displayName)
description := "test description"
requestBody.SetDescription(&description)
options := &msgraphsdk.ProgramsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Programs().Post(options)


```