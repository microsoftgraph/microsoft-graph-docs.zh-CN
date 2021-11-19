---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f17b37077d1877c69e5c342f6d46d2ddae18ba6b
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61103542"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

contactFolderId := "contactFolder-id"
result, err := graphClient.Me().ContactFoldersById(&contactFolderId).ChildFolders().Get(options)


```