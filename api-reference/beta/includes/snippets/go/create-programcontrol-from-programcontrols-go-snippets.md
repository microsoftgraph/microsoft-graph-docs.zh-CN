---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 771d0407ded41e8476b94c094f612d1a3dcf862c
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61086894"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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