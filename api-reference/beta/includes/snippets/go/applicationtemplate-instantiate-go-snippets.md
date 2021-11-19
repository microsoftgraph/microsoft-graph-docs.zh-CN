---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e365d090ef63848dd32e25bac754085783297333
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61089516"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
displayName := "My custom name"
requestBody.SetDisplayName(&displayName)
options := &msgraphsdk.InstantiateRequestBuilderPostOptions{
    Body: requestBody,
}
applicationTemplateId := "applicationTemplate-id"
result, err := graphClient.ApplicationTemplatesById(&applicationTemplateId).Instantiate().Post(options)


```