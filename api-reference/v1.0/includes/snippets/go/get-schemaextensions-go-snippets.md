---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 64e261c6a666ed853301d0b2f5f21fcc6a90bede
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61091511"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.SchemaExtensionsRequestBuilderGetQueryParameters{
    Filter: "id%20eq%20'graphlearn_test'",
}
options := &msgraphsdk.SchemaExtensionsRequestBuilderGetOptions{
    Q: requestParameters,
}
result, err := graphClient.SchemaExtensions().Get(options)


```