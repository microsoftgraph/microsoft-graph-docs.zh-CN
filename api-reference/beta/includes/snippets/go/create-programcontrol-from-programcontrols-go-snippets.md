---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e1f25e18e9b9ab63fa89006cbbbf90b66c6aa3b1
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65314936"
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
result, err := graphClient.ProgramControls().Post(requestBody)


```