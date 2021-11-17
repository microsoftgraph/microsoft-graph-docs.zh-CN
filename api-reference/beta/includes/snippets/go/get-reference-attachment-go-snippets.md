---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 19566ed8126f2b124d025913300d3874247f535b
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60982532"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

eventId := "event-id"
attachmentId := "attachment-id"
result, err := graphClient.Me().EventsById(&eventId).AttachmentsById(&attachmentId).Get(options)


```