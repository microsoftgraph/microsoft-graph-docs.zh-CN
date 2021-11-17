---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 78706e7f155d82520694f82310610b93db8f4ac6
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61021019"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

chatId := "chat-id"
result, err := graphClient.ChatsById(&chatId).PermissionGrants().Get(options)


```