---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a38d6cc6bc8517510386d5c3019aa82fc24380f6
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61029734"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

eventId := "event-id"
attachmentId := "attachment-id"
graphClient.Me().EventsById(&eventId).AttachmentsById(&attachmentId).Delete(options)


```