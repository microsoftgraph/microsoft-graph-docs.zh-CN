---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 850b0ec6bc6e64f7957b6a8b1123372d817eb331
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61026703"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

groupId := "group-id"
conversationThreadId := "conversationThread-id"
result, err := graphClient.GroupsById(&groupId).ThreadsById(&conversationThreadId).Posts().Get(options)


```