---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 22b39e37b502eae8f70140ca4cc9276febada8e5
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61093054"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.OrgContactRequestBuilderGetQueryParameters{
    Select: "displayName,jobTitle,mail",
}
options := &msgraphsdk.OrgContactRequestBuilderGetOptions{
    Q: requestParameters,
}
orgContactId := "orgContact-id"
result, err := graphClient.ContactsById(&orgContactId).Get(options)


```