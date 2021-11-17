---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c1b7a9917f76ced144dbb7ac1d0de7281b2f8424
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61023139"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

messageId := "message-id"
extensionId := "extension-id"
graphClient.Me().MessagesById(&messageId).ExtensionsById(&extensionId).Delete(options)


```