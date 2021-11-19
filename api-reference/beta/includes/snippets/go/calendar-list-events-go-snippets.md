---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 941b519cced44d9e229543e3bbfc4586a3ac644a
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61088565"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.EventsRequestBuilderGetQueryParameters{
    Filter: "startsWith(subject,'All')",
}
options := &msgraphsdk.EventsRequestBuilderGetOptions{
    Q: requestParameters,
}
result, err := graphClient.Me().Calendar().Events().Get(options)


```