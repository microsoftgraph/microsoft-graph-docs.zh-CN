---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0e906857af163b3bf140159a8c31d9d567dacbc5
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61086328"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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