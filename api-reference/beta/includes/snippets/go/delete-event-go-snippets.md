---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a2a55e1c0ce41675cd9063ee7a66a1bfe89b2b32
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61030161"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

eventId := "event-id"
graphClient.Me().EventsById(&eventId).Delete(options)


```