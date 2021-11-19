---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 87369d3f5c98e39b034859a17cef6aa26c1aec15
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61100408"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.PoliciesRequestBuilderGetQueryParameters{
    Filter: "displayName%20eq%20'SimplePolicy1'%20or%20displayName%20eq%20'SimplePolicy2'",
}
options := &msgraphsdk.PoliciesRequestBuilderGetOptions{
    Q: requestParameters,
}
result, err := graphClient.Identity().ConditionalAccess().Policies().Get(options)


```