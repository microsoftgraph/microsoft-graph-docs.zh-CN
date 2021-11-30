---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 24656e933a49fc8ed69ef9f0715829d78add5786
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/30/2021
ms.locfileid: "61225509"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.AttributeSetsRequestBuilderGetQueryParameters{
    Top: 10,
}
options := &msgraphsdk.AttributeSetsRequestBuilderGetOptions{
    Q: requestParameters,
}
result, err := graphClient.Directory().AttributeSets().Get(options)


```