---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4ddb9c5624e612b1803308acca284c8735e1a9a0
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61095664"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.ProfileRequestBuilderGetQueryParameters{
    Expand: "names($select=first,last),skills($select=displayName)",
}
options := &msgraphsdk.ProfileRequestBuilderGetOptions{
    Q: requestParameters,
}
result, err := graphClient.Me().Profile().Get(options)


```