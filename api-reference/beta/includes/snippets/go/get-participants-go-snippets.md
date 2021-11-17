---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1879b017391352e4428dd3a1ba10a0e7ccaf95bf
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61019975"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

callId := "call-id"
result, err := graphClient.Communications().CallsById(&callId).Participants().Get(options)


```