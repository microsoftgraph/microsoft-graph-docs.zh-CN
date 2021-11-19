---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 76c4da0d9d30f78d6d76228cd47ec84d6ef9198a
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61102906"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

setId := "set-id"
graphClient.TermStore().SetsById(&setId).Delete(options)


```