---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 39ad369ae2831ce94da71474493a9aed0bf99db8
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61032121"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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