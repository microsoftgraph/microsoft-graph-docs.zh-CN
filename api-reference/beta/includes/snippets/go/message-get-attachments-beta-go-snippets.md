---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c6c43f8965de5b94af3bff790081e5574aa37962
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61028300"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

messageId := "message-id"
result, err := graphClient.Me().MessagesById(&messageId).Attachments().Get(options)


```