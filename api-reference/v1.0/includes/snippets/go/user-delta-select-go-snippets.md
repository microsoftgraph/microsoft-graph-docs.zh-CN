---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7f4350cc82406d5358a27a1587e69662abc94335
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62137611"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.DeltaRequestBuilderGetQueryParameters{
    Select: "displayName,jobTitle,mobilePhone",
}
options := &msgraphsdk.DeltaRequestBuilderGetOptions{
    Q: requestParameters,
}
result, err := graphClient.Users().Delta()().Get(options)


```