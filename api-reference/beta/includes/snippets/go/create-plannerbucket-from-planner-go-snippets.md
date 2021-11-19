---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f1ee825345fef3875479947f499ed4332a6b5ed1
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61084456"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewPlannerBucket()
name := "Advertising"
requestBody.SetName(&name)
planId := "xqQg5FS2LkCp935s-FIFm2QAFkHM"
requestBody.SetPlanId(&planId)
orderHint := " !"
requestBody.SetOrderHint(&orderHint)
options := &msgraphsdk.BucketsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Planner().Buckets().Post(options)


```