---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 020e36bdccb12a76037ac73f54d6e1c255a74435
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61026541"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

userId := "user-id"
outlookTaskId := "outlookTask-id"
result, err := graphClient.UsersById(&userId).Outlook().TasksById(&outlookTaskId).Attachments().Get(options)


```