---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fe6667ae0f36c78be17492ddd09df191c5baf65e
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63393373"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.GroupsRequestBuilderGetQueryParameters{
    Select: "id,assignedLicenses",
    Filter: "assignedLicenses/any()",
}
options := &msgraphsdk.GroupsRequestBuilderGetOptions{
    Q: requestParameters,
}
result, err := graphClient.Groups().Get(options)


```