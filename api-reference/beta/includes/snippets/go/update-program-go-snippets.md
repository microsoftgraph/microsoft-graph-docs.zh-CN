---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c941cb5d2e1be2849d5e779776e793d374a8a34c
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61007354"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewProgram()
displayName := "testprogram3 new name"
requestBody.SetDisplayName(&displayName)
options := &msgraphsdk.ProgramRequestBuilderPatchOptions{
    Body: requestBody,
}
programId := "program-id"
graphClient.ProgramsById(&programId).Patch(options)


```