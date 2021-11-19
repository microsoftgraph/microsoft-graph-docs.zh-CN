---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3a749add449cfb269265f5d30c61541520978f5f
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61098091"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

outlookTaskId := "outlookTask-id"
graphClient.Me().Outlook().TasksById(&outlookTaskId).Delete(options)


```