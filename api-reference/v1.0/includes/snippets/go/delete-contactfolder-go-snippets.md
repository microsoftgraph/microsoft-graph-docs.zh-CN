---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fd80b953e8bc764bfcd21f91b0049937bdc0df2b
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61096970"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

contactFolderId := "contactFolder-id"
graphClient.Me().ContactFoldersById(&contactFolderId).Delete(options)


```