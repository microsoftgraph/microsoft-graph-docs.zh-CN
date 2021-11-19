---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a9a667b16a9af869a34b89883d939fdbe53f5824
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61101889"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.MailFoldersRequestBuilderGetQueryParameters{
    IncludeHiddenFolders: true,
}
options := &msgraphsdk.MailFoldersRequestBuilderGetOptions{
    Q: requestParameters,
}
result, err := graphClient.Me().MailFolders().Get(options)


```