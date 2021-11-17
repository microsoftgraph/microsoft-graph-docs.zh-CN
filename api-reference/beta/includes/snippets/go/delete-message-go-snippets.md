---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6bbf7c913355724f7785872e388635b226c76daf
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60980846"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

messageId := "message-id"
graphClient.Me().MessagesById(&messageId).Delete(options)


```