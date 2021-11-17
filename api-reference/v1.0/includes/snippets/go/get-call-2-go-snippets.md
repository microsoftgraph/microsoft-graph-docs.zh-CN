---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5bac7278ee5a9f29fa4f0cabda5dfb6051589548
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60974537"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

callId := "call-id"
result, err := graphClient.Communications().CallsById(&callId).Get(options)


```