---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8e63218edfec3123f2ffd4938254d61c36a3447b
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60974522"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

callId := "call-id"
graphClient.Communications().CallsById(&callId).Delete(options)


```