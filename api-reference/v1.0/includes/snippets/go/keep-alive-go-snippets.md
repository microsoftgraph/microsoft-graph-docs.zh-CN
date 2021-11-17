---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f70106eb63481392699b4f15792376ab6fae650b
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60974452"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

callId := "call-id"
graphClient.Communications().CallsById(&callId).KeepAlive().Post(options)


```