---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 79a2246aa7853866ba0852ee6da3543ec049ec2c
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62115550"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewTiIndicator()
description := "description-updated"
requestBody.SetDescription(&description)
options := &msgraphsdk.TiIndicatorRequestBuilderPatchOptions{
    Body: requestBody,
}
tiIndicatorId := "tiIndicator-id"
graphClient.Security().TiIndicatorsById(&tiIndicatorId).Patch(options)


```