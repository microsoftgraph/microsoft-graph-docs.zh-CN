---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cfc12123cd2650efc19cef238f8a31b3618e21ea
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60993647"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.ContactRequestBuilderGetQueryParameters{
    Select: "displayName",
}
headers := map[string]string{
    "Prefer": "odata.maxpagesize=2"
}
options := &msgraphsdk.ContactRequestBuilderGetOptions{
    Q: requestParameters,
    H: headers,
}
contactFolderId := "contactFolder-id"
contactId := "contact-id"
result, err := graphClient.Me().ContactFoldersById(&contactFolderId).ContactsById(&contactId).Get(options)


```