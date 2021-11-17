---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0b20601ff015e6337ad9cf2329b92d9bded73bd3
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61027865"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewProgramControl()
controlId := "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213"
requestBody.SetControlId(&controlId)
controlTypeId := "6e4f3d20-c5c3-407f-9695-8460952bcc68"
requestBody.SetControlTypeId(&controlTypeId)
programId := "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213"
requestBody.SetProgramId(&programId)
options := &msgraphsdk.ProgramControlsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.ProgramControls().Post(options)


```