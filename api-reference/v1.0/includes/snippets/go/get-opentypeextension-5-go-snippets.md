---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 690f0921dbc6ddfe6d8b26f022a48594734295b7
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61097217"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.MessagesRequestBuilderGetQueryParameters{
    Filter: "Extensions/any(f:f/id%20eq%20'Com.Contoso.Referral')",
    Expand: "Extensions($filter=id%20eq%20'Com.Contoso.Referral')",
}
options := &msgraphsdk.MessagesRequestBuilderGetOptions{
    Q: requestParameters,
}
result, err := graphClient.Me().Messages().Get(options)


```