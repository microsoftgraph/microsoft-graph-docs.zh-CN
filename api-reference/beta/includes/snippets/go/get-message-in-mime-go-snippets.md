---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 062124090e52a584e12be704744d60672d429a3a
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61028333"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

messageId := "message-id"
graphClient.Me().MessagesById(&messageId).$value().Get(options)


```