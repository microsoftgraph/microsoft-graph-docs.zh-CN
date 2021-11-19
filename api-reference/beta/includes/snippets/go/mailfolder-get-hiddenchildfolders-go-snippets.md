---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5d40beaa9915fe21f13238a7378ec5f573773976
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61094038"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.ChildFoldersRequestBuilderGetQueryParameters{
    IncludeHiddenFolders: true,
}
options := &msgraphsdk.ChildFoldersRequestBuilderGetOptions{
    Q: requestParameters,
}
mailFolderId := "mailFolder-id"
result, err := graphClient.Me().MailFoldersById(&mailFolderId).ChildFolders().Get(options)


```