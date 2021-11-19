---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cce7e656012dfc3b6c827fb0c470ccd471f60511
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61104227"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

headers := map[string]string{
    "Prefer": "odata.maxpagesize=2"
}
options := &msgraphsdk.ContactFolderRequestBuilderGetOptions{
    H: headers,
}
contactFolderId := "contactFolder-id"
result, err := graphClient.Me().ContactFoldersById(&contactFolderId).Get(options)


```