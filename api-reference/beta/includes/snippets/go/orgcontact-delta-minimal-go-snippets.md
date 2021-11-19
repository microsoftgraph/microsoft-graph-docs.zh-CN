---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 79dafa6ef6b04275ea6f52f817594b994cfac9a1
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61095333"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.OrgContactRequestBuilderGetQueryParameters{
    Select: "displayName,jobTitle,mail",
}
headers := map[string]string{
    "Prefer": "return=minimal"
}
options := &msgraphsdk.OrgContactRequestBuilderGetOptions{
    Q: requestParameters,
    H: headers,
}
orgContactId := "orgContact-id"
result, err := graphClient.ContactsById(&orgContactId).Get(options)


```