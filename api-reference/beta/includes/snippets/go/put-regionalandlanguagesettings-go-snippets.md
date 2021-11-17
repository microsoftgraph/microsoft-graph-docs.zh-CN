---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4f221bd9da4fe7058a9044233458401040ac138d
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60996883"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "authoringLanguages":  []Object {
    }
}
options := &msgraphsdk.RegionalAndLanguageSettingsRequestBuilderPutOptions{
    Body: requestBody,
}
graphClient.Me().Settings().RegionalAndLanguageSettings().Put(options)


```