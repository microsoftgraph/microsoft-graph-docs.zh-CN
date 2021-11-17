---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 908b169f240639a5abace64e6504d2e1282540db
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60987292"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

callId := "call-id"
graphClient.Communications().CallsById(&callId).Transfer().Post(options)


```