---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cb679484af03e483660d3e894e07360491179a11
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61004904"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

eventId := "event-id"
result, err := graphClient.Me().EventsById(&eventId).Attachments().Get(options)


```