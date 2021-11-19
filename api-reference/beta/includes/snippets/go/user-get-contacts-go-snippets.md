---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e8a3eea594d5778fc51bc9bd375a6804745c0560
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61100665"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.ContactsRequestBuilderGetQueryParameters{
    Select: "displayName,emailAddresses",
}
options := &msgraphsdk.ContactsRequestBuilderGetOptions{
    Q: requestParameters,
}
result, err := graphClient.Me().Contacts().Get(options)


```